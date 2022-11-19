# SandboxSound
------------------------------------------------------------------------------------------
## 描述

一个发出声音的对象

*继承自*：
* [SandboxNode](/Api/Class/SandBoxNode.md)

------------------------------------------------------------------------------------------
## 属性：

|<div style="width:1125px">[string](/Api/DataType/String.md) &emsp; [<font color="dd00dd">SoundPath</font>](/Api/Class/Sound/SandboxSound_F/SoundPath.md)</div>|
|:---|
|声音资源路径|

|<div style="width:1125px">[Button]() &emsp; [<font color="dd00dd">Play</font>](/Api/Class/Sound/SandboxSound_F/Play.md)</div>|
|:---|
|试听(`EDITORUI::Button`)|

|<div style="width:1125px">[float](/Api/DataType/Float.md) &emsp; [<font color="dd00dd">Volume</font>](/Api/Class/Sound/SandboxSound_F/Volume.md)</div>|
|:---|
|声音音量大小|

|<div style="width:1125px">[bool](/Api/DataType/Bool.md) &emsp; [<font color="dd00dd">IsLoop</font>](/Api/Class/Sound/SandboxSound_F/IsLoop.md)</div>|
|:---|
|设置该声音是否重复播放|

|<div style="width:1125px">[bool](/Api/DataType/Bool.md) &emsp; [<font color="dd00dd">IsPlaying</font>](/Api/Class/Sound/SandboxSound_F/IsPlaying.md)</div>|
|:---|
|仅在脚本可获取，用于标识声音是否完成播放（暂停但未完成播放也为true）|

|<div style="width:1125px">[bool](/Api/DataType/Bool.md) &emsp; [<font color="dd00dd">IsPaused</font>](/Api/Class/Sound/SandboxSound_F/IsPaused.md)</div>|
|:---|
|仅在脚本可获取，用于标识声音是否处于暂停状态|

|<div style="width:1125px">[bool](/Api/DataType/Bool.md) &emsp; [<font color="dd00dd">PlayOnRemove</font>](/Api/Class/Sound/SandboxSound_F/PlayOnRemove.md)</div>|
|:---|
|设置为true时，会在移除节点后播放一次声音|

|<div style="width:1125px">[bool](/Api/DataType/Bool.md) &emsp; [<font color="dd00dd">NeedRelease</font>](/Api/Class/Sound/SandboxSound_F/NeedRelease.md)</div>|
|:---|
|设置为true时，标记为会被释放|

|<div style="width:1125px">[SandboxNode](/Api/Class/SandBoxNode.md) &emsp; [<font color="dd00dd">TransObject</font>](/Api/Class/Sound/SandboxSound_F/TransObject.md)</div>|
|:---|
|设置为某个`SceneTransObject`节点后，`Sound`将在该节点的位置播放（3D声音），若`TransObject`与`FixPos`均未设置，则为全局播放（2D声音）|

|<div style="width:1125px">[Vector3](/Api/DataType/Vector3.md) &emsp; [<font color="dd00dd">FixPos</font>](/Api/Class/Sound/SandboxSound_F/FixPos.md)</div>|
|:---|
|设置后，若没有指定`TransObject`，则在指定位置(`Rainbow::Vector3f`)播放3D声音|

|<div style="width:1125px">[bool](/Api/DataType/Bool.md) &emsp; [<font color="dd00dd">IsFixPosPlay</font>](/Api/Class/Sound/SandboxSound_F/IsFixPosPlay.md)</div>|
|:---|
|只可读，为true时代表正在`FixPos`属性所指位置播放3D声音|

|<div style="width:1125px">[EnumRollOffMode](/Api/Enumerate/Sound/EnumRollOffMode.md) &emsp; [<font color="dd00dd">RollOffMode</font>](/Api/Class/Sound/SandboxSound_F/RollOffMode.md)</div>|
|:---|
|声音衰减模式，包括逆衰减（默认），线性衰减，线性平方衰减，锥型逆衰减模式。见枚举`EnumRollOffMode`|

|<div style="width:1125px">[float](/Api/DataType/Float.md) &emsp; [<font color="dd00dd">RollOffMaxDistance</div>](/Api/Class/Sound/SandboxSound_F/RollOffMaxDistance.md)|
|:---|
|声音衰减最大距离|

|<div style="width:1125px">[float](/Api/DataType/Float.md) &emsp; [<font color="dd00dd">RollOffMinDistance</div>](/Api/Class/Sound/SandboxSound_F/RollOffMinDistance.md)|
|:---|
|声音衰减最小距离|

------------------------------------------------------------------------------------------

## 函数：

|<div style="width:925px">[void](/Api/Parameter/void.md)&emsp;[<font color="dd00dd">PlaySound</font>](/Api/Class/Sound/SandboxSound_F/PlaySound.md)( )</div>|
|:---|
|播放/继续播放声音（调用后IsPlaying为true，IsPaused为false）|


|<div style="width:925px">[void](/Api/Parameter/void.md)&emsp;[<font color="dd00dd">StopSound</font>](/Api/Class/Sound/SandboxSound_F/StopSound.md)( )</div>|
|:---|
|停止播放声音（调用后IsPlaying为false）|



|<div style="width:925px">[void](/Api/Parameter/void.md)&emsp;[<font color="dd00dd">ResumeSound</font>](/Api/Class/Sound/SandboxSound_F/ResumeSound.md)( )</div>|
|:---|
|重新播放声音（声音将从头开始播放）|



|<div style="width:925px">[void](/Api/Parameter/void.md)&emsp;[<font color="dd00dd">PauseSound</font>](/Api/Class/Sound/SandboxSound_F/PauseSound.md)( )</div>|
|:---|
|暂停声音（调用后IsPaused为true）|


------------------------------------------------------------------------------------------
## 事件：

|<div style="width:925px">[SBXSignal](/Api/Parameter/void.md)&emsp;[<font color="dd00dd">PlayFinish</font>](/Api/Class/Sound/SandboxSound_F/PlayFinish.md)( [SandboxNode](/Api/Class/SandBoxNode.md) node)</div>|
|:---|
|`SandboxSound`实例播放结束时触发该事件|


------------------------------------------------------------------------------------------
## 示例代码：

```lua
local part = script.Parent --获取父节点
local sound1 = SandboxNode.new('SandboxSound', part) --创建Sound节点
sound1.SoundPath ="sandboxSysId://sounds/npc/chest.ogg" --设置资源路径
sound1.TransObject = script.Parent --绑定TransObject（播放3D声音）
sound1.IsLoop = true --设置循环播放
sound1.PlayOnRemove = true --设置移除时播放
sound1.RollOffMode = Enum.EnumRollOffMode.Linear --设置声音衰减模式
sound1.RollOffMinDistance = 300
sound1.RollOffMaxDistance = 700
sound1:PlaySound() --播放函数

--播放结束事件
sound1.PlayFinish:connect(function(node) 
    node:Destroy()
    print("sound is Destroy")
end)
```