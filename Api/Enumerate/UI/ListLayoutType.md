# ListLayoutType

枚举所属类：[SceneUIImage](/Api/Class/Scene/SceneUIImage.md) 

------------------------------------------------------------------------------------------
## 描述

排列方式，需要与[OverflowType](/Api/Enumerate/UI/OverflowType.md)配套使用才有效果

------------------------------------------------------------------------------------------
## 枚举

|<div style="width:200px">ListLayoutType</div>|<div style="width:100px"></div>|<div style="width:100px"></div>|
|:---   |:---|:---|
|**名称**   |**值**  |**描述**|
|SINGLE_COLUMN   |0   |单列，每行一个item，竖向排列。|
|SINGLE_ROW|1   |单行，每列一个item，横向排列。|
|FLOW_HORIZONTAL  |2   |横向流动，item横向依次排列，到底视口右侧边缘或到达指定的列数，自动换行继续排列。|
|FLOW_VERTICAL  |3   |竖向流动，item竖向依次排列，到底视口底部边缘或到达指定的行数，返回顶部开启新的一列继续排列。|
|PAGINATION  |4   |分页，视口宽度x视口高度作为单页大小，横向排列各个页面。每页中，item横向依次排列|