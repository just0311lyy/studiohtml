# DefaultEffect
------------------------------------------------------------------------------------------
## 描述

特效节点，可以用于播放一个特效

*继承自*：
* [SceneTransObject](/Api/Class/NoType/SceneTransObject.md)

------------------------------------------------------------------------------------------
## 属性

|<div style="width:1000px">[EnumDefaultEffect](/Api/Enumerate/Effect/EnumDefaultEffect.md) &emsp;[<font color="dd00dd">EffectType</font>]()</div>|
|:---|
|特效效果类型,有烟雾、爆炸、光效、粒子、火焰、环境和提示。见枚举`SandboxDefaultEffect::`[EnumDefaultEffect](/Api/Enumerate/Effect/EnumDefaultEffect.md)|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">EffectIndex</font>]()</div>|
|:---|
|特效效果序列|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">Scale</font>]()</div>|
|:---|
|效果大小, 整体缩放比例|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">Visible</font>]()</div>|
|:---|
|是否显示视觉效果|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">MaxTime</font>]()</div>|
|:---|
|效果最大存在时间|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">VisibleDistance</font>]()</div>|
|:---|
|效果最大可见距离|

------------------------------------------------------------------------------------------
## 函数

------------------------------------------------------------------------------------------
## 示例代码

```lua
local workspace = game:GetService("workspace")
local Effect = SandboxNode.new('SandboxDefaultEffect', workspace)
local pos2 = Vector3.new(unpack({1000,1000,1000}))
--设置特效位置
Effect.Position = pos2
--设置特效为火焰类型
Effect.EffectType = Enum.EnumDefaultEffect.Fire
--设置特效序列
Effect.EffectIndex = 13
--设置特效时长
Effect.MaxTime = 10
--设置特效可见距离
Effect.VisibleDistance = 100
 ```