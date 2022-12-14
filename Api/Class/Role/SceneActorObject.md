# Actor
------------------------------------------------------------------------------------------
## 描述

*继承自*：
* [SceneModelObject](/Api/Class/Role/SceneModelObject.md)

------------------------------------------------------------------------------------------
## 属性：

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">Movespeed</font>](/Api/Class/Role/SceneActorObject_F/Movespeed.md)</div>|
|:---|
|生物的移动速度|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">MaxHealth</font>](/Api/Class/Role/SceneActorObject_F/MaxHealth.md)</div>|
|:---|
|生物的最大生命值|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">Health</font>](/Api/Class/Role/SceneActorObject_F/Health.md)</div>|
|:---|
|生物的当前生命值|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">UseCameraAngle</font>](/Api/Class/Role/SceneActorObject_F/UseCameraAngle.md)</div>|
|:---|
|是否使用相机角度|

|<div style="width:1000px">[BehaviorState](/Api/Enumerate/Role/BehaviorState.md) &emsp;[<font color="dd00dd">MoveState</font>](/Api/Class/Role/SceneActorObject_F/MoveState.md)</div>|
|:---|
|行为状态枚举，见枚举[BehaviorState](/Api/Enumerate/Role/BehaviorState.md)|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">UserId</font>](/Api/Class/Role/SceneActorObject_F/UserId.md)</div>|
|:---|
|用户id|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">NoPath</font>](/Api/Class/Role/SceneActorObject_F/NoPath.md)</div>|
|:---|
|是否无导航路径|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">SetGravity</font>](/Api/Class/Role/SceneActorObject_F/SetGravity.md)</div>|
|:---|
|重力|

------------------------------------------------------------------------------------------
## 函数

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetMoveEndTime</font>](/Api/Class/Role/SceneActorObject_F/SetMoveEndTime.md) ([float](/Api/DataType/Float.md) endtime)</div>|
|:---|
|设置生物移动的结束时间|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">MoveTo</font>](/Api/Class/Role/SceneActorObject_F/MoveTo.md) ([Vector3](/Api/DataType/Vector3.md) target)</div>|
|:---|
|移动到某个位置|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">Move</font>](/Api/Class/Role/SceneActorObject_F/SetMoveEndTime.md) ([Vector3](/Api/DataType/Vector3.md) dir, [bool](/Api/DataType/Bool.md) relativeToCamera)</div>|
|:---|
|朝某个方向移动|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">Jump</font>](/Api/Class/Role/SceneActorObject_F/Jump.md) ([bool](/Api/DataType/Bool.md) jump)</div>|
|:---|
|设置生物是否跳跃|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetJumpInfo</font>](/Api/Class/Role/SceneActorObject_F/SetJumpInfo.md) ([float](/Api/DataType/Float.md) baseSpeed, [float](/Api/DataType/Float.md) continueSpeed)</div>|
|:---|
|设置生物跳跃参数|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">NavigateTo</font>](/Api/Class/Role/SceneActorObject_F/NavigateTo.md) ([Vector3](/Api/DataType/Vector3.md) target)</div>|
|:---|
|寻路到某个位置|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetOneJumpTick</font>](/Api/Class/Role/SceneActorObject_F/SetOneJumpTick.md) ([int](/Api/DataType/Int.md) tickcount)</div>|
|:---|
|设置一个跳跃行为|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetEnableContinueJump</font>](/Api/Class/Role/SceneActorObject_F/SetEnableContinueJump.md) ([bool](/Api/DataType/Bool.md) enable)</div>|
|:---|
|设置是否能连续跳跃|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">StopNavigate</font>](/Api/Class/Role/SceneActorObject_F/StopNavigate.md) ()</div>|
|:---|
|停止寻路|

|<div style="width:1000px">[BehaviorState](/Api/Enumerate/Role/BehaviorState.md) &emsp;[<font color="dd00dd">GetCurMoveState</font>](/Api/Class/Role/SceneActorObject_F/GetCurMoveState.md) ()</div>|
|:---|
|获取当前行为状态。见枚举[BehaviorState](/Api/Enumerate/Role/BehaviorState.md)|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">UseDefaultAnimation</font>](/Api/Class/Role/SceneActorObject_F/UseDefaultAnimation.md) ([bool](/Api/DataType/Bool.md) use)</div>|
|:---|
|移动过程中使用默认的动作|

------------------------------------------------------------------------------------------
## 事件

|<div style="width:500px">[SBXSignal\<bool\>]() &emsp;[<font color="dd00dd">Walking</font>](/Api/Class/Role/SceneActorObject_F/Walking.md) ()</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|生物行走时触发（返回值有可能为空）||||
|**返回类型**|||**概要**|
|SBXSignal|||生物行走时触发，事件参数为（`bool isWalking`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|isWalking|bool||行走是否触发|


|<div style="width:500px">[SBXSignal\<bool\>]() &emsp;[<font color="dd00dd">Standing</font>](/Api/Class/Role/SceneActorObject_F/Standing.md) ()</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|生物站立时触发（返回值有可能为空）||||
|**返回类型**|||**概要**|
|SBXSignal|||生物站立时触发，事件参数为（`bool isStanding`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|isStanding|bool||站立是否触发|

|<div style="width:500px">[SBXSignal\<bool\>]() &emsp;[<font color="dd00dd">Jumping</font>](/Api/Class/Role/SceneActorObject_F/Jumping.md) ()</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|生物跳跃时触发（返回值有可能为空）||||
|**返回类型**|||**概要**|
|SBXSignal|||生物跳跃时触发，事件参数为（`bool isJumping`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|isJumping|bool||跳跃是否触发|

|<div style="width:500px">[SBXSignal\<bool\>]() &emsp;[<font color="dd00dd">Flying</font>](/Api/Class/Role/SceneActorObject_F/Flying.md) ()</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|生物飞行时触发（返回值有可能为空）||||
|**返回类型**|||**概要**|
|SBXSignal|||生物飞行时触发，事件参数为（`bool isFlying`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|isFlying|bool||飞行是否触发|

|<div style="width:500px">[SBXSignal\<bool\>]() &emsp;[<font color="dd00dd">Died</font>](/Api/Class/Role/SceneActorObject_F/Died.md) ()</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|生物死亡时触发（返回值有可能为空）||||
|**返回类型**|||**概要**|
|SBXSignal|||生物死亡时触发，事件参数为（`bool isDied`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|isDied|bool||死亡是否触发|

|<div style="width:500px">[SBXSignal\<BehaviorState, BehaviorState\>]() &emsp;[<font color="dd00dd">MoveStateChange</font>](/Api/Class/Role/SceneActorObject_F/MoveStateChange.md) ()</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|生物行为改变时触发，从一个行为改为另外一个行为||||
|**返回类型**|||**概要**|
|SBXSignal|||生物行为改变时触发，事件参数为（`BehaviorState beforeState, BehaviorState afterState`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|beforeState|BehaviorState||改变前的行为|
|afterState|BehaviorState||改变后的行为|

|<div style="width:500px">[SBXSignal\<bool\>]() &emsp;[<font color="dd00dd">AvigateFinished</font>](/Api/Class/Role/SceneActorObject_F/AvigateFinished.md) ()</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|寻路结束时触发（返回值有可能为空）||||
|**返回类型**|||**概要**|
|SBXSignal|||生物寻路结束时触发，事件参数为（`bool isAvigateFinished`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|isAvigateFinished|bool||寻路结束是否触发|


|<div style="width:500px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;[<font color="dd00dd">MoveFinished</font>](/Api/Class/Role/SceneActorObject_F/MoveFinished.md) ()</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|移动MoveTo结束后触发||||
|**返回类型**|||**概要**|
|SBXSignal|||移动`MoveTo`结束后触发|

|<div style="width:500px">[SBXSignal\<bool\>]() &emsp;[<font color="dd00dd">MoveFinished待定</font>](/Api/Class/Role/SceneActorObject_F/MoveFinished.md) ()</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|移动`MoveTo`结束后触发（返回值有可能为空）||||
|**返回类型**|||**概要**|
|SBXSignal|||生物移动结束时触发，事件参数为（`bool isMoveFinished`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|isMoveFinished|bool||移动MoveTo结束后触发|


------------------------------------------------------------------------------------------
## 示例代码

```
--创建实例
local newActor = SandboxNode.new('SceneActorObject')
--设置名字
newActor.Name = "my_actor"
--设置模型
newActor.ModelId = string.format("sandboxAsset://entity/%s/body.omod","100010")
--设置位置
newActor.Position = Vector3.new(500,700,500)
--设置父节点
newActor:SetParent(Workspace)
--设置速度
newActor.Movespeed = 2 
--监听MoveFineshed事件
newActor.MoveFinished:connect(function(isMoveFinished)
        print("actor move:"..tostring(isMoveFinished))
end)

newActor.Walking:connect(function()
        print("actor walking..")
end)
```