# DefaultSound
------------------------------------------------------------------------------------------
## 描述

音效节点，可以用于原生库中的音效（在`Sound.csv`中配置的音效）<br>
继承：`SandboxSound`

------------------------------------------------------------------------------------------
## 属性

|<div style="width:925px">[EnumDefaultSound](/Api/Enumerate/Sound/EnumDefaultSound.md)&emsp;[<font color="dd00dd">SoundType</font>](/Api/Class/Sound/SandboxDefaultSound_F/SoundType.md)</div>|
|:---|
|默认声音类型枚举：脚步、行为、受击、待机、技能、环境、背景音乐、提示和其他。见枚举[EnumDefaultSound](/Api/Enumerate/Sound/EnumDefaultSound.md)|

|<div style="width:925px"> [int](/Api/DataType/Int.md)&emsp;[<font color="dd00dd">EffectIndex</font>](/Api/Class/Sound/SandboxDefaultSound_F/EffectIndex.md)</div>|
|:---|
|音效效果序列|


------------------------------------------------------------------------------------------
## 函数

------------------------------------------------------------------------------------------
## 示例代码

```lua
 local workspace = game:GetService("workspace")
 local Effect = SandboxNode.new('SandboxDefaultSound', part)
 --设置音效为脚步
 Effect.SoundType = Enum.EnumDefaultSound.FootStep
 --设置音效序列
 Effect.EffectIndex = 13
 Effect:PlaySound() --播放音效
 ```