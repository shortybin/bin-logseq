- flex 分为容器和 item
- 容器主要的属性：
- ```
  flex-direction: 设置容器内 item 的排列方向
  flex-wrap: 设置容器内 item 是否换行
  justify-content: 沿 Flex 容器的主轴分配 Flex 容器的剩余空间
  align-content：沿 Flex 容器的侧轴分配 Flex 容器的剩余空间
  align-items：将所有 Flex 项目作为一个组，沿 Flex 容器侧轴对齐
  ```
- item 主要的属性：
- ```
  order: 定义 item 的排序，数值越小越靠前
  flex-grow: item 的放大比例，类似 Android 中 LinearLayout 的 weight
  flex-shrik: item 的缩小比例，设置为 0 则不缩放
  align-self: item 的对齐方式，可覆盖 align-items 属性
  ```
- 默认情况下，item 在侧轴上会被拉伸伸展，因为 Flex 容器 align-items 属性的默认值为 stretch
- 当容器没有足够大的空间来存放所有的子元素时，子元素会按照一定的压缩率被压缩，这个压缩率就是由flex-shrink来设置（flex-shrink默认值为1），可以设置 flex-shrink 为0不压缩。