# UIList
------------------------------------------------------------------------------------------
## 描述

`UI`列表组件

*继承自*：
* [SceneUIComponent](/Api/Class/Scene/SceneUIComponent.md)

------------------------------------------------------------------------------------------
## 属性

|<div style="width:1000px">[OverflowType](/Api/Enumerate/UI/OverflowType.md) &emsp;[<font color="dd00dd">OverflowType</font>](/Api/Class/Scene/SceneUIList_F/OverflowType.md)</div>|
|:---|
|溢出处理，设置`ScrollType`时，需要将该属性同步修改（如设置横向流动，此处需设置`HORIZONTAL`）才能达到效果，包括以下几种：<br>溢出部分正常显示（无拖动效果）;<br>溢出部分隐藏（无拖动效果）;<br>水平滚动，支持鼠标拖拽，滑轮方式水平拖动;<br>垂直滚动，支持鼠标拖拽，滑轮方式垂直拖动;<br>自由滚动，支持鼠标拖拽，滑轮方式任意方向拖动<br>参见枚举`SceneUIList::`[OverflowType](/Api/Enumerate/UI/OverflowType.md)|

|<div style="width:1000px">[ListLayoutType](/Api/Enumerate/UI/ListLayoutType.md) &emsp;[<font color="dd00dd">ScrollType</font>](/Api/Class/Scene/SceneUIList_F/ScrollType.md)</div>|
|:---|
|排列方式，需要与[OverflowType](/Api/Enumerate/UI/OverflowType.md)配套使用才有效果，包括以下几种：<br>单列，每行一个item，竖向排列;<br>单行，每列一个item，横向排列;<br>横向流动，item横向依次排列，到底视口右侧边缘或到达指定的列数，自动换行继续排列;<br>竖向流动，item竖向依次排列，到底视口底部边缘或到达指定的行数，返回顶部开启新的一列继续排列;<br>分页，视口宽度x视口高度作为单页大小，横向排列各个页面。每页中，item横向依次排列<br>参见枚举`fairygui::`[ListLayoutType](/Api/Enumerate/UI/ListLayoutType.md)|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">LineCount</font>](/Api/Class/Scene/SceneUIList_F/LineCount.md)</div>|
|:---|
|行数|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">ColumnCount</font>](/Api/Class/Scene/SceneUIList_F/ColumnCount.md)</div>|
|:---|
|列数|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">LineGap</font>](/Api/Class/Scene/SceneUIList_F/LineGap.md)</div>|
|:---|
|行距|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">ColumnGap</font>](/Api/Class/Scene/SceneUIList_F/ColumnGap.md)</div>|
|:---|
|列距|

|<div style="width:1000px">[TextHAlignment](/Api/Enumerate/UI/TextHAlignment.md) &emsp;[<font color="dd00dd">HorizontalAlign</font>](/Api/Class/Scene/SceneUIList_F/HorizontalAlign.md)</div>|
|:---|
|水平对齐方式，有以下几种：<br>靠左对齐;<br>居中对齐;<br>靠右对齐<br>参见枚举`cocos2d::TextHAlignment`|

|<div style="width:1000px">[TextVAlignment](/Api/Enumerate/UI/TextVAlignment.md) &emsp;[<font color="dd00dd">VerticalAlign</font>](/Api/Class/Scene/SceneUIList_F/VerticalAlign.md)</div>|
|:---|
|垂直对齐方式，有以下几种：<br>向上对齐;<br>居中对齐;<br>向下对齐;<br>参见枚举`cocos2d::TextVAlignment`|


|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">AutoResizeItem</font>](/Api/Class/Scene/SceneUIList_F/AutoResizeItem.md)</div>|
|:---|
|自动调整列表项目大小，如果勾选:<br>列表布局为单列，则列表项目的宽度自动设置为列表显示区域的宽度；<br>列表布局为单行，则列表项目的高度自动设置为列表显示区域的高度；<br>列表布局为水平流动，且设置了列数时，则每行内的列表项目的宽度自动调整使行宽与列表显示区域的宽度相等；<br>列表布局为垂直流动，且设置了行数时，则每列内的项目的高度自动调整使行高与列表显示区域的高度相等；<br>列表布局为分页，则3、4规则均适用;<br>参见枚举`fairygui::`[ListLayoutType](/Api/Enumerate/UI/ListLayoutType.md)|


------------------------------------------------------------------------------------------
## 函数

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetVirtual</font>](/Api/Class/Scene/SceneUIList_F/FontSize.md)( )</div>|
|:---|
|设置虚拟列表，只为可视范围内的item创建实体对象（不可取消）|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetVirtualAndLoop</font>](/Api/Class/Scene/SceneUIList_F/FontSize.md)( )</div>|
|:---|
|设置循环列表（同时也是虚拟列表），头尾相接（不可取消）|

------------------------------------------------------------------------------------------
## 示例代码

```lua
local workspace = game:GetService("Workspace")
local name = SandboxNode.new('SceneUIList', workspace)

--设置排列方式
name.ScrollType = Enum.ListLayoutType.FLOW_HORIZONTAL
name.OverflowType = Enum.OverflowType.HORIZONTAL 
--设置行数列数
name.LineCount = 2
name.ColumnCount = 2

--设置行距列距
name.LineGap= 50
name.ColumnGap= 50

--设置自动调整项目大小
name.AutoResizeItem= true

--设置上下居中对齐
name.HorizontalAlign= Enum.TextVAlignment.Center
--设置左右向左对齐
name.VerticalAlign= Enum.TextHAlignment.Left

--设置虚拟循环列表
name.SetVirtualAndLoop
```