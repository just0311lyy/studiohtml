# HingeJoint
------------------------------------------------------------------------------------------
## 描述

铰链类型的连接点

*继承自*：
* [SandboxJoint](/Api/Class/Bind/SandboxJoint.md)

------------------------------------------------------------------------------------------
## 属性

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">LimitsEnable</font></div>|
|:---|
|是否限制启用|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">EffectType（不可用，已删除）</font>]()</div>|
|:---|
|是否限制旋转角度|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;<font color="dd00dd">UpperAngle</font></div>|
|:---|
|限制的最大角度|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;<font color="dd00dd">LowerAngle</font></div>|
|:---|
|限制的最小角度|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;<font color="dd00dd">Restitution</font></div>|
|:---|
|达到最大或最小角度后的一个回拉力|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;<font color="dd00dd">Spring</font></div>|
|:---|
|弹力|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;<font color="dd00dd">Damping</font></div>|
|:---|
|阻尼大小|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;<font color="dd00dd">LimitTargetAngle</font></div>|
|:---|
|目标角度|

|<div style="width:1000px">[/Api/Enumerate/Physics/MotorType]() &emsp;<font color="dd00dd">ActuatorType</font></div>|
|:---|
|传动类型（传动类型为：`MOTOR`时 ），见枚举`MotorType`|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;<font color="dd00dd">MotorAngularSpeed</font></div>|
|:---|
|角速度|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;<font color="dd00dd">MotorMaxTorque</font></div>|
|:---|
|最大扭矩 ——暂时还没实现。传动类型为：`SERVO`时|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">ServoAngularSpeed（不可用，已删除）</font>]()</div>|
|:---|
|角速度|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">ServoMaxTorque（不可用，已删除）</font>]()</div>|
|:---|
|最大扭矩|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">ServoTargetAngle（不可用，已删除）</font>]()</div>|
|:---|
|目标角度|


------------------------------------------------------------------------------------------
## 函数



------------------------------------------------------------------------------------------
## 示例代码

```lua
local workspace = game:GetService("workspace")
--创建一个物理模型
local model1 = SandboxNode.new('SceneModelObject', workspace)
local model2 = SandboxNode.new('SceneModelObject', workspace)
--在两个模型下面分别添加一个附着点
local att0 = SandboxNode.new('SandboxAttachmentObject', model1)
local att1 = SandboxNode.new('SandboxAttachmentObject', model2)
--在其中一个模型下面添加一个连接点
local HingeJoint = SandboxNode.new('SandboxHingeJoint', model1)
--给连接点绑定两个模型的附着点
HingeJoint.attachment0 = att0
HingeJoint.attachment1 = att1
--是否设置最大角度
HingeJoint.LimitsEnable = true
--设置两种不同传动类型
HingeJoint.ActuatorType = Enum.MotorType.MOTOR
```