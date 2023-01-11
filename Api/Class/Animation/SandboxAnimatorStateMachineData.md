# AnimatorStateMachineData
------------------------------------------------------------------------------------------
## 描述

Animator 状态机数据

*继承自*：
* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md)

------------------------------------------------------------------------------------------
## 属性

------------------------------------------------------------------------------------------
## 函数

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp; <font color="dd00dd">Clear</font> ()</div>|
|:---|
|清空持有的Asset和清空加载|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsValid</font>](/Api/Class/Animation/SandboxAnimatorStateMachineData_F/IsValid.md) ()</div>|
|:---|
|检测是否已经失效了（底层数据已经失效了）|

|<div style="width:1000px"> vector<[AnimatorStateMachineData](/Api/Class/Animation/SandboxAnimatorStateMachineData.md)> &emsp;[<font color="dd00dd">GetSubMachines</font>](/Api/Class/Animation/SandboxAnimatorStateMachineData_F/GetSubMachines.md) ()</div>|
|:---|
|获取当前持有的子状态机数据|

|<div style="width:1000px"> vector<[AnimatorStateData](/Api/Class/Animation/SandboxAnimatorStateData.md)> &emsp;[<font color="dd00dd">GetStates</font>](/Api/Class/Animation/SandboxAnimatorStateMachineData_F/GetStates.md) ()</div>|
|:---|
|获取当前持有的所有状态数据|

|<div style="width:1000px"> [AnimatorStateData](/Api/Class/Animation/SandboxAnimatorStateData.md) &emsp;[<font color="dd00dd">CreateState</font>](/Api/Class/Animation/SandboxAnimatorStateMachineData_F/CreateState.md) ([string](/Api/DataType/String.md) name)</div>|
|:---|
|创建一个状态数据|

|<div style="width:1000px"> [AnimatorStateData](/Api/Class/Animation/SandboxAnimatorStateData.md) &emsp;[<font color="dd00dd">GetState</font>](/Api/Class/Animation/SandboxAnimatorStateMachineData_F/GetState.md) ([string](/Api/DataType/String.md) name)</div>|
|:---|
|获取一个状态数据|

------------------------------------------------------------------------------------------
## 事件


------------------------------------------------------------------------------------------
## 示例代码

```lua
```