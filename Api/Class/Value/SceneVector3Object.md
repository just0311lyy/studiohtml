# SceneVector3Object
------------------------------------------------------------------------------------------
## 描述
 
继承：`SandboxNode` 
------------------------------------------------------------------------------------------
## 属性

|<div style="width:1125px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">Value</font>](/Api/Class/Value/SceneVector3Object_F/Value.md)</div>|
|:---|
|用于存储`Vector3`|

------------------------------------------------------------------------------------------
## 事件
 
|<div style="width:500px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;[<font color="dd00dd">ValueChanged</font> ](/Api/Class/Value/SceneVector3Object_F/ValueChanged.md) ( [Vector3](/Api/DataType/Vector3.md) Value)</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|当`vector3value`改变时，通知值已更改||||
|**返回类型**|||**概要**|
|SBXSignal|||进入`vector3value`改变时触发，事件参数为（`Vector3 vector3value`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|vector3value|Vector3||当`vector3value`改变时，通知值已更改|

------------------------------------------------------------------------------------------
## 示例代码

```lua
local workspace = game:GetService("workspace")
local vec = SandboxNode.new('SceneVector3Object', workspace)
vec.Value.x = 1
vec.Value.y = 1
vec.Value.z = 1
```