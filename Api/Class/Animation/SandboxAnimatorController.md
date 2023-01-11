# AnimatorController
------------------------------------------------------------------------------------------
## 描述

Animator Controller 数据

*继承自*：
* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md)

------------------------------------------------------------------------------------------
## 属性

------------------------------------------------------------------------------------------
## 函数

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp; <font color="dd00dd">Clear</font> ()</div>|
|:---|
|清空持有的Asset和清空加载|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsValid</font>](/Api/Class/Animation/SandboxAnimatorController_F/IsValid.md) ()</div>|
|:---|
|检测是否已经失效了（底层数据已经失效了）|

|<div style="width:1000px"> [int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">GetStateMachineCount</font>](/Api/Class/Animation/SandboxAnimatorController_F/GetStateMachineCount.md) ()</div>|
|:---|
|获取当前持有的状态机个数|

|<div style="width:1000px"> [AnimatorStateMachineData](/Api/Class/Animation/SandboxAnimatorStateMachineData.md) &emsp;[<font color="dd00dd">GetStateMachine</font>](/Api/Class/Animation/SandboxAnimatorController_F/GetStateMachine.md) ([int](/Api/DataType/Int.md) index)</div>|
|:---|
|按照`layer`获取当前的状态机实例|

|<div style="width:1000px"> [AnimatorLayerData](/Api/Class/Animation/SandboxAnimatorLayerData.md) &emsp;[<font color="dd00dd">CreateLayer</font>](/Api/Class/Animation/SandboxAnimatorController_F/CreateLayer.md) ([string](/Api/DataType/String.md) name)</div>|
|:---|
|新建一个AnimatorLayerData实例|

------------------------------------------------------------------------------------------
## 事件


------------------------------------------------------------------------------------------
## 示例代码

```lua
```