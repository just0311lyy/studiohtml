# Area
------------------------------------------------------------------------------------------
## 描述

*继承自*：
* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md)

------------------------------------------------------------------------------------------
## 属性

|<div style="width:1000px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">Beg</font>](/Api/Class/GamePlay/AreaNode_F/Beg.md)</div>|
|:---|
|起始位置世界坐标|

|<div style="width:1000px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">End</font>](/Api/Class/GamePlay/AreaNode_F/End.md)</div>|
|:---|
|结束位置世界坐标|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">EffectWidth</font>](/Api/Class/GamePlay/AreaNode_F/EffectWidth.md)</div>|
|:---|
|效果宽度|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">Show</font>](/Api/Class/GamePlay/AreaNode_F/Show.md)</div>|
|:---|
|是否显示|

|<div style="width:1000px">[SHOWMODE]() &emsp;[<font color="dd00dd">ShowMode</font>](/Api/Class/GamePlay/AreaNode_F/ShowMode.md)</div>|
|:---|
|显示模式的枚举(`SceneEffectFrame::SHOWMODE`):<br>X = 1,<br>Y = 2,<br>Z = 4,<br>XY = 1+2,<br>XZ = 1+4,<br>YZ = 2+4,<br>XYZ = 1+2+4|


|<div style="width:1000px">[ColorValue](/Api/DataType/ColourValue.md) &emsp;[<font color="dd00dd">Color</font>](/Api/Class/GamePlay/AreaNode_F/Color.md)</div>|
|:---|
|设置区域颜色|

------------------------------------------------------------------------------------------
## 事件

|<div style="width:500px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;[<font color="dd00dd">NotifyEnterNode</font>](/Api/Class/GamePlay/AreaNode_F/NotifyEnterNode.md) ( [SandboxNode](/Api/Class/NoType/SandboxNode.md) node )</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|节点进入该区域||||
|**返回类型**|||**概要**|
|SBXSignal|||进入节点时触发，事件参数为（`SandboxNode node`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|node|SandboxNode||进入该区域的`SandboxNode`节点|

|<div style="width:500px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;[<font color="dd00dd">NotifyLeaveNode</font>](/Api/Class/GamePlay/AreaNode_F/NotifyLeaveNode.md) ( [SandboxNode](/Api/Class/NoType/SandboxNode.md) node  )</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|节点离开该区域||||
|**返回类型**|||**概要**|
|SBXSignal|||离开节点时触发，事件参数为（`SandboxNode node`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|node|SandboxNode||离开该区域的`SandboxNode`节点|

------------------------------------------------------------------------------------------
## 示例代码：

```lua
local part = script.Parent --获取父节点
local area = SandboxNode.new('AreaNode', part) --创建AreaNode节点

--创建Actor实例
local actorNode = SandboxNode.new('SceneActorObject')
actorNode.Name = "my_actor"

--actorNode进入区域
area.NotifyEnterNode:connect(function(actorNode) 
    print("actorNode进入区域")
end)
```