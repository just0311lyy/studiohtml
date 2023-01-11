# UITextLabel
------------------------------------------------------------------------------------------
## 描述

一个`text`文本组件

*继承自*：
* [SceneUIComponent](/Api/Class/Scene/SceneUIComponent.md)

------------------------------------------------------------------------------------------
## 属性：

|<div style="width:1000px">[ColorValue](/Api/DataType/colorValue.md) &emsp;<font color="dd00dd">TitleColor</font></div>|
|:---|
|字体颜色  (`Rainbow::ColorQuad`)|

|<div style="width:1000px">[TextVAlignment](/Api/Enumerate/UI/TextVAlignment.md) &emsp;<font color="dd00dd">TextVAlignment</font></div>|
|:---|
|上下对齐，有向上、中间和向下对齐。参见枚举`cocos2d::`[TextVAlignment](/Api/Enumerate/UI/TextVAlignment.md)|

|<div style="width:1000px">[TextHAlignment](/Api/Enumerate/UI/TextHAlignment.md) &emsp;<font color="dd00dd">TextHAlignment</font></div>|
|:---|
|左右对齐，有向左、中间和向右对齐。参见枚举`cocos2d::`[TextHAlignment](/Api/Enumerate/UI/TextHAlignment.md)|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;<font color="dd00dd">FontSize</font></div>|
|:---|
|字体大小|

|<div style="width:1000px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">Title</font></div>|
|:---|
|文本内容|

|<div style="width:1000px">[AutoSizeType](/Api/Enumerate/UI/AutoSizeType.md) &emsp;<font color="dd00dd">IsAutoSize</font></div>|
|:---|
|自动调整节点大小为字体大小。参见枚举`fairygui::`[AutoSizeType](/Api/Enumerate/UI/AutoSizeType.md)|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">OutlineEnable</font></div>|
|:---|
|开启描边|

|<div style="width:1000px">[ColorValue](/Api/DataType/colorValue.md) &emsp;<font color="dd00dd">OutlineColor</font></div>|
|:---|
|描边颜色 (`Rainbow::ColorQuad`)|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;<font color="dd00dd">OutlineSize</font></div>|
|:---|
|描边宽度|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">ShadowEnable</font></div>|
|:---|
|开启阴影|

|<div style="width:1000px">[ColorValue](/Api/DataType/colorValue.md) &emsp;<font color="dd00dd">ShadowColor</font></div>|
|:---|
|阴影颜色|

|<div style="width:1000px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">ShadowOffect</font></div>|
|:---|
|阴影偏移  (`Rainbow::Vector2f`)|

------------------------------------------------------------------------------------------
## 函数

|<div style="width:500px">[Vector2](/Api/DataType/Vector2.md) &emsp;[<font color="dd00dd">GetTextSize</font> ]() ()</div>|<div style="width:698px"></div>|
|:---|:---|
|获取字体大小||
|**返回类型**|**概要**|
|Vector2|返回`text`尺寸|

------------------------------------------------------------------------------------------
## 示例代码：

```lua
local workspace = game:GetService("Workspace")
local root = SandboxNode.new('SceneUIRoot', workspace)
local name = SandboxNode.new('SceneUITextLabel', root)
name.Title = "商店"
--设置背景框
name.LineColor = ColorValue.new(0, 0, 0, 0)
--设置背景颜色
name.FillColor = ColorValue.new(0, 0, 0, 0)
--设置字体颜色
name.TitleColor = ColorValue.new(255, 0, 0, 255)
--设置位置
name.Position = Vector2.new(75,50)
--设置字体大小
name.FontSize = 18
--设置上下居中对齐
name.TextVAlignment = Enum.TextVAlignment.Center
--设置左右向左对齐
name.TextHAlignment = Enum.TextHAlignment.Left

--设置自动调整大小
name.IsAutoSize= true

--设置开启描边
name.OutlineEnable= true
--设置开启阴影
name.ShadowEnable= true
--获取字体大小
local size = name:GetTextSize()
```