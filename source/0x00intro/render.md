# 渲染


## 简介
 
渲染引擎解析 HTML 文档，并将各标记逐个转化成 DOM 节点。同时也会解析外部 CSS 文件以及样式元素中的样式数据。

## Render树
 
- Render树包含若干带有颜色、面积等可视化属性的矩形
- 矩形按照在屏幕上展现的顺序排列
- 并不是所有DOM树的节点都有对应的Render树，不可见元素就没有在Render树中

## 构建流程
 
- 根节点在处理HTML中的body标签时构建，其余部分随DOM节点插入而构建
- 样式计算：计算每一个渲染对象的可视化属性
    - 按照连接序应用样式规则
    - 继承规则
    - 赋默认值
- 根据目标媒介，生成渲染对象
    - 屏幕：visual flow 模型
    - 可打印设备：page 模型
    - 语音渲染设备：aural rendering 模型

## 布局过程
 
- 赋予每一个Render树节点在屏幕中出现的准确坐标
- 采用流模型（从左到右 从上到下）
- 坐标系的原点在左上
- 采用全局和增量式布局
    - 全局样式改变影响局部渲染
    - 变化的矩形被重新布局
