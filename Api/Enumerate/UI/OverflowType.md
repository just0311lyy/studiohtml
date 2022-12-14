# OverflowType

枚举所属类：[UIImage](/Api/Class/Scene/SceneUIImage.md) 

------------------------------------------------------------------------------------------
## 描述

溢出处理，设置`ScrollType`时，需要将该属性同步修改（如设置横向流动，此处需设置`HORIZONTAL`）才能达到效果

------------------------------------------------------------------------------------------
## 枚举

|<div style="width:200px">OverflowType</div>|<div style="width:100px"></div>|<div style="width:100px"></div>|
|:---   |:---|:---|
|**名称**   |**值**  |**描述**|
|VISIBLE   |0   |溢出部分正常显示（无拖动效果）|
|HIDDEN|1   |溢出部分隐藏（无拖动效果）|
|HORIZONTAL  |2   |水平滚动，支持鼠标拖拽，滑轮方式水平拖动|
|VERTICAL  |3   |垂直滚动，支持鼠标拖拽，滑轮方式垂直拖动
|BOTH  |4   |自由滚动，支持鼠标拖拽，滑轮方式任意方向拖动|