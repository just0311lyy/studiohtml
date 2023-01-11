# UIComponent
------------------------------------------------------------------------------------------
## 描述

`UI`约束和布局类别的基类，由[SceneUIBase](/Api/Class/Scene/SceneUIBase.md)继承而来

*继承自*：
* [SceneUIBase](/Api/Class/Scene/SceneUIBase.md)

------------------------------------------------------------------------------------------
## 属性

|<div style="width:1000px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">Size</font></div>|
|:---|
|UI节点像素和尺寸大小 (`Rainbow::Vector2f`)|

|<div style="width:1000px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">Scale</font></div>|
|:---|
|UI节点缩放倍数|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;<font color="dd00dd">Rotation</font></div>|
|:---|
|UI节点旋转度数|

|<div style="width:1000px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">Position</font></div>|
|:---|
|UI节点坐标|

|<div style="width:1000px">[Vector2](/Api/DataType/Vector2.md) &emsp;<font color="dd00dd">Pivot</font></div>|
|:---|
|UI节点锚点（0~1），（0.5,0.5）为中点|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">IsKeepPosWhenPivotChange</font></div>|
|:---|
|更新锚点时是否保持位置不变|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">IsNotifyEventStop</font></div>|
|:---|
|是否将触摸事件传递给父节点（为true时不传递）|

|<div style="width:1000px">[ColorValue](/Api/DataType/colorValue.md) &emsp;<font color="dd00dd">LineColor</font></div>|
|:---|
|UI节点边线颜色设置 (Rainbow::ColorQuad)|

|<div style="width:1000px">[ColorValue](/Api/DataType/colorValue.md) &emsp;<font color="dd00dd">FillColor</font></div>|
|:---|
|UI节点填充颜色设置|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;<font color="dd00dd">LineSize</font></div>|
|:---|
|UI节点边线像素和尺寸大小|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">ClickPass</font></div>|
|:---|
|UI节点边线像素和尺寸大小|

|<div style="width:1000px">[EnumLayoutHRelation](/Api/Enumerate/UI/EnumLayoutHRelation.md) &emsp;<font color="dd00dd">LayoutHRelation</font></div>|
|:---|
|水平关联方式，包括左关联、中线关联和右关联。设置后，当父节点（若父节点为[`UIRoot`](/Api/Class/Scene/SceneUIRoot.md)则为屏幕）变化时，UI与关联位置的相对距离将保持不变。<br>参见枚举[EnumLayoutHRelation](/Api/Enumerate/UI/EnumLayoutHRelation.md)|

|<div style="width:1000px">[EnumLayoutVRelation](/Api/Enumerate/UI/EnumLayoutVRelation.md) &emsp;<font color="dd00dd">LayoutVRelation</font></div>|
|:---|
|垂直关联方式，包括上关联、中线关联和下关联。设置后，当父节点（若父节点为[`UIRoot`](/Api/Class/Scene/SceneUIRoot.md)则为屏幕）变化时，UI与关联位置的相对距离将保持不变。<br>参见枚举[EnumLayoutVRelation](/Api/Enumerate/UI/EnumLayoutVRelation.md)|

|<div style="width:1000px">[EnumLayoutSizeRelation](/Api/Enumerate/UI/EnumLayoutSizeRelation.md) &emsp;<font color="dd00dd">LayoutSizeRelation</font></div>|
|:---|
|宽高关联，包括无关联，宽关联，高关联和全关联，当父节点宽高改变时，UI宽高随之变化。<br>参见枚举[EnumLayoutSizeRelation](/Api/Enumerate/UI/EnumLayoutSizeRelation.md)|


------------------------------------------------------------------------------------------
## 函数

|<div style="width:500px">[Vector2](/Api/DataType/Vector2.md) &emsp;[<font color="dd00dd">GetGlobalPos</font>](/Api/Class/Scene/SceneUIComponent_F/GetGlobalPos.md) ()</div>|
|:---|
|获取UI的全局位置|

------------------------------------------------------------------------------------------
## 事件

|<div style="width:500px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;<font color="dd00dd">RollOver</font> ( [SandboxNode](/Api/Class/NoType/SandboxNode.md) node, [bool](/Api/DataType/Bool.md) isOver, [Vector2](/Api/DataType/Vector2.md) mousePosition)</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|拖住滑动或鼠标滚轮结束||||
|**返回类型**|||**概要**|
|SBXSignal|||进入节点时触发，事件参数为（`SandboxNode node, bool, Vector2`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|node|SandboxNode||当前`ui`节点组件|
|isOver|bool||是否正拖住鼠标或者鼠标滚轮结束|
|vector2|Vector2||当前鼠标的二维坐标(`Rainbow::Vector2f`)|


|<div style="width:500px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;<font color="dd00dd">RollOut</font> ( [SandboxNode](/Api/Class/NoType/SandboxNode.md) node , [bool](/Api/DataType/Bool.md)isOut , [Vector2](/Api/DataType/Vector2.md) mousePosition )</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|拖住滑动或鼠标滚轮超出UI布局范围||||
|**返回类型**|||**概要**|
|SBXSignal|||进入节点时触发，事件参数为（`SandboxNode node, bool, Vector2`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|node|SandboxNode||当前`ui`节点组件|
|isOut|bool||是否拖住滑动或鼠标滚轮超出UI布局范围|
|vector2|Vector2||当前鼠标的二维坐标(`Rainbow::Vector2f`)|

|<div style="width:500px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;<font color="dd00dd">TouchBegin</font> ( [SandboxNode](/Api/Class/NoType/SandboxNode.md) node, [bool](/Api/DataType/Bool.md)isTouchBegin, [Vector2](/Api/DataType/Vector2.md) mousePosition )</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|触摸事件开始||||
|**返回类型**|||**概要**|
|SBXSignal|||进入节点时触发，事件参数为（`SandboxNode node, bool, Vector2`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|node|SandboxNode||当前`ui`节点组件|
|isTouchBegin|bool||是否触摸事件开始|
|vector2|Vector2||当前鼠标的二维坐标(`Rainbow::Vector2f`)|

|<div style="width:500px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;<font color="dd00dd">TouchMove</font> ( [SandboxNode](/Api/Class/NoType/SandboxNode.md) node, [bool](/Api/DataType/Bool.md)isTouchMove, [Vector2](/Api/DataType/Vector2.md) mousePosition)</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|触摸移动||||
|**返回类型**|||**概要**|
|SBXSignal|||进入节点时触发，事件参数为（`SandboxNode node, bool, Vector2`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|node|SandboxNode||当前`ui`节点组件|
|isTouchMove|bool||是否触摸移动|
|vector2|Vector2||当前鼠标的二维坐标(`Rainbow::Vector2f`)|

|<div style="width:500px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;<font color="dd00dd">TouchEnd</font> ( [SandboxNode](/Api/Class/NoType/SandboxNode.md) node, [bool](/Api/DataType/Bool.md)isTouchEnd, [Vector2](/Api/DataType/Vector2.md) mousePosition)</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|触摸事件结束||||
|**返回类型**|||**概要**|
|SBXSignal|||进入节点时触发，事件参数为（`SandboxNode node, bool, Vector2`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|node|SandboxNode||当前`ui`节点组件|
|isTouchEnd|bool||是否触摸事件结束|
|vector2|Vector2||当前鼠标的二维坐标(`Rainbow::Vector2f`)|


|<div style="width:500px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;<font color="dd00dd">Click</font> ( [SandboxNode](/Api/Class/NoType/SandboxNode.md) node, [bool](/Api/DataType/Bool.md)isClick, [Vector2](/Api/DataType/Vector2.md) mousePosition))</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|点击事件||||
|**返回类型**|||**概要**|
|SBXSignal|||进入节点时触发，事件参数为（`SandboxNode node, bool, Vector2`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|node|SandboxNode||当前`ui`节点组件|
|isClick|bool||是否点击事件|
|vector2|Vector2||当前鼠标的二维坐标(`Rainbow::Vector2f`)|

------------------------------------------------------------------------------------------
## 示例代码

```lua
--创建ui布局
local root = SandboxNode.new('SceneUIRoot', game.WorkSpace)
root.Name = 'uiroot'
--创建图片
local image1 = SandboxNode.new('SceneUIImage', game.WorkSpace.uiroot)
image1.Name = 'image'
image1.Visible = true
image1.Icon = 'ui\\mobile\\texture0\\common\\board_activity_box_white.png'
image1.Size = Vector2.new(500, 200)
image1.Pivot= Vector2.new(0, 0)
image1.LayoutHRelation = Enum.EnumLayoutHRelation.Left
image1.LayoutVRelation= Enum.EnumLayoutVRelation.Top
image1.LayoutSizeRelation= Enum.EnumLayoutSizeRelation.Both

image1.RollOver:connect(function(node,issuccess,mousepos) 
    print('you RollOver me')
    print('RollOver pos:'..mousepos.x..' '..mousepos.y)
end)
image1.RollOut:connect(function(node,issuccess,mousepos) 
    print('you RollOut me')
    print('RollOut pos:'..mousepos.x..' '..mousepos.y)
end)
image1.TouchBegin:connect(function(node,issuccess,mousepos) 
    print('you TouchBegin me')
    print('TouchBegin pos:'..mousepos.x..' '..mousepos.y)
end)
image1.TouchMove:connect(function(node,issuccess,mousepos) 
    print('you TouchMove me')
    print('TouchMove pos:'..mousepos.x..' '..mousepos.y)
end)
image1.TouchEnd:connect(function(node,issuccess,mousepos) 
    print('you TouchEnd me')
    print('TouchEnd pos:'..mousepos.x..' '..mousepos.y)
end)
image1.Click:connect(function(node,issuccess,mousepos) 
    print('you Clickme')
    print('Clickme pos:'..mousepos.x..' '..mousepos.y)
end)
```