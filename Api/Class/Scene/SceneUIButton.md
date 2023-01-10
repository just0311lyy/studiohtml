# UIButton
------------------------------------------------------------------------------------------
## 描述

*继承自*：
* [SceneUIComponent](/Api/Class/Scene/SceneUIComponent.md)

------------------------------------------------------------------------------------------
## 属性

|<div style="width:1000px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">Icon</font>](/Api/Class/Scene/SceneUIButton_F/Icon.md)</div>|
|:---|
|按钮资源路径|

|<div style="width:1000px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">Title</font>](/Api/Class/Scene/SceneUIButton_F/Title.md)</div>|
|:---|
|按钮标题|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">TitleSize</font>](/Api/Class/Scene/SceneUIButton_F/TitleSize.md)</div>|
|:---|
|按钮标题文本字体大小|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">DownEffectValue</font>](/Api/Class/Scene/SceneUIButton_F/DownEffectValue.md)</div>|
|:---|
|按钮按下效果变化值|

|<div style="width:1000px">[DownEffect]() &emsp;[<font color="dd00dd">DownEffect</font>](/Api/Class/Scene/SceneUIButton_F/DownEffect.md)</div>|
|:---|
|按钮按下效果，有缩放，颜色变化。参见枚举`DownEffect` (`SceneUIButton::ButtonDownEffect`)|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">Alpha</font>](/Api/Class/Scene/SceneUIButton_F/Alpha.md)</div>|
|:---|
|透明度（0~1） 为1时不透明|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">OutlineEnable</font>](/Api/Class/Scene/SceneUIButton_F/OutlineEnable.md)</div>|
|:---|
|开启字体描边|

|<div style="width:1000px">[ColorValue](/Api/DataType/colorvalue.md) &emsp;[<font color="dd00dd">OutlineColor</font>](/Api/Class/Scene/SceneUIButton_F/OutlineColor.md)</div>|
|:---|
|字体描边颜色  (`Rainbow::ColorQuad`)|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">OutlineSize</font>](/Api/Class/Scene/SceneUIButton_F/OutlineSize.md)</div>|
|:---|
|字体描边宽度|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">ShadowEnable</font>](/Api/Class/Scene/SceneUIButton_F/ShadowEnable.md)</div>|
|:---|
|开启字体阴影|

|<div style="width:1000px">[ColorValue](/Api/DataType/colorvalue.md) &emsp;[<font color="dd00dd">ShadowColor</font>](/Api/Class/Scene/SceneUIButton_F/ShadowColor.md)</div>|
|:---|
|字体阴影颜色  (`Rainbow::ColorQuad`)|

|<div style="width:1000px">[Vector2](/Api/DataType/Vector2.md) &emsp;[<font color="dd00dd">ShadowOffect</font>](/Api/Class/Scene/SceneUIButton_F/ShadowOffect.md)</div>|
|:---|
|字体阴影偏移 (`Rainbow::Vector2f`)|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsAutoSize</font>](/Api/Class/Scene/SceneUIButton_F/IsAutoSize.md)</div>|
|:---|
|自动大小。为`true`时，将节点大小调整为图片原本大小|

------------------------------------------------------------------------------------------


------------------------------------------------------------------------------------------
## 函数


------------------------------------------------------------------------------------------
## 示例代码

```lua
--创建ui布局
local root = SandboxNode.new('SceneUIRoot', game.WorkSpace)
root.Name = 'uiroot'
--创建按钮
local button= SandboxNode.new('SceneUIButton', game.WorkSpace.uiroot)
button.Icon = 'ui\\mobile\\texture0\\common\\board_activity_box_white.png'
button.Title = "Button"
button.TitleSize = 36
button.DownEffect = Enum.DownEffect.ScaledEffect
button.Size = Vector2.new(100, 50)
button.Position = Vector2.new(200, 100)
button.Alpha= 1
--设置开启描边
button.OutlineEnable= true
--设置开启阴影
button.ShadowEnable= true
```