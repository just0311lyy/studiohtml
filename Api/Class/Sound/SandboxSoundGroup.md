# SoundGroup
------------------------------------------------------------------------------------------
#### 描述

声音分组节点，统一控制声音的播放，停止，音量等（请直接将声音节点挂在SoundGroup节点下面，`SoundGroup->Node->Sound`的挂载方式将不会起到控制效果）

*继承自*：
*  [`SandBoxNode`](/Api/Class/NoType/SandboxNode.md)

------------------------------------------------------------------------------------------
## 属性：

------------------------------------------------------------------------------------------
## 函数：

|<div style="width:925px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">PlaySound</font> ](/Api/Class/Sound/SandboxSoundGroup_F/PlaySound)( )</div>|
|:-----------------------|
|播放/继续播放组内声音            |



|<div style="width:925px">[void](/Api/Parameter/void.md)  &emsp;[<font color="dd00dd">StopSound</font> ](/Api/Class/Sound/SandboxSoundGroup_F/StopSound)( )</div>|
|:---|
|停止播放组内声音|

|<div style="width:925px">[void](/Api/Parameter/void.md)  &emsp;[<font color="dd00dd">ResumeSound</font> ](/Api/Class/Sound/SandboxSoundGroup_F/ResumeSound)( )</div>|
|:---|
|重新播放组内声音（声音将从头开始播放）|

|<div style="width:925px">[void](/Api/Parameter/void.md)  &emsp;[<font color="dd00dd">PauseSound</font> ](/Api/Class/Sound/SandboxSoundGroup_F/PauseSound)( )</div>|
|:---|
|暂停组内声音|

|<div style="width:925px">[void](/Api/Parameter/void.md)  &emsp;[<font color="dd00dd">ChangeVolume</font> ](/Api/Class/Sound/SandboxSoundGroup_F/ChangeVolume.md)( [float](/Api/DataType/Float.md) vaval)</div>|
|:---|
|按比例改变组内声音音量（0~1），如：传入0.5会将组内Sound节点音量减半|

------------------------------------------------------------------------------------------
## 事件：

------------------------------------------------------------------------------------------
## 示例代码：

```lua
	local part = script.Parent --获取父节点
	local soundGroup = SandboxNode.new('SandboxSoundGroup', part) --创建Sound节点
	soundGroup:ChangeVolume(0.5) --按比例调节音量
	soundGroup:PlaySound() --播放
	soundGroup:StopSound() --停止
```