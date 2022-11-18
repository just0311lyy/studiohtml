# SceneIntObject
------------------------------------------------------------------------------------------
## 描述
 
继承：`SandboxNode` 
------------------------------------------------------------------------------------------
## 属性：

|<div style="width:1125px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">Value</font>](/Api/Class/Value/SceneIntObject_F/Value.md)</div>|
|:---|
|用于存储int。|

------------------------------------------------------------------------------------------
## 事件：

|<div style="width:500px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;[<font color="dd00dd">ValueChanged</font> ](/Api/Class/Value/SceneIntObject_F/ValueChanged.md) ( [int](/Api/DataType/Int.md) Value)</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|当`intvalue`改变时，通知值已更改||||
|**返回类型**|||**概要**|
|SBXSignal|||进入`intvalue`改变时触发，事件参数为（`int intvalue`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|intvalue|int||当`intvalue`改变时，通知值已更改|
 
------------------------------------------------------------------------------------------
## 示例代码：

```lua
local workspace = game:GetService("workspace")
local i = SandboxNode.new('SceneIntObject', workspace)
i.Value = 1
```