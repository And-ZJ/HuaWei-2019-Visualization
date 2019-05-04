## 2019 华为软件精英挑战赛 地图可视化

### 源信息

基于 https://github.com/AkatsukiCC/huawei2019-with-visualization 魔改而来。

主要魔改：降低了绘制时间，修改了显示内容，自己的坐标计算方式。

### 文件说明

#### CrossCoordinate.py

通过road.txt 和 cross.txt 建立地图坐标。用于指导绘制位置。（这里不是像素坐标，仅仅只是各路口在坐标系中的位置）

此文件额外实现了跨节点绘制道路。（默认道路是不会跨路口的，即路口(0,0)和(0,2)，若有道路直连，则属于跨节点情况，虽然最后没有考到这种情况）

#### CoordinateFileOper.py

文本形式的坐标标记

#### MapVisualization.py

核心

实现地图绘制。

#### TestCrossCoordinate.py

测试文件

若改动了CrossCoordinate.py文件的计算方式，使用此文件确保几张奇怪地图的坐标计算结果正确。

#### TimeTools.py

计算运行时间

##### map-strange-\*目录

这里均是存在跨节点的地图

其他地图来自官方






