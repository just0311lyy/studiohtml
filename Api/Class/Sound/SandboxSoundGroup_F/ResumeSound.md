# ResumeSound
-----------------------------------------------------------------------------------------
## 描述

函数所属类：[SandboxSoundGroup](/Api/Class/Sound/SandboxSoundGroup.md)

重新播放，会将声音组内所有声音重头开始播放

| 设置音源是否循环大小等参数需要对相应的声音节点进行设置

-----------------------------------------------------------------------------------------
## 参数


无参数


## 返回

无返回值

------------------------------------------------------------------------------------------
## 示例代码：

```lua
local part = script.Parent --获取父节点
local soundGroup = SandboxNode.new('SandboxSoundGroup', part) --创建Sound节点
soundGroup:ChangeVolume(0.5) --按比例调节音量
soundGroup:PlaySound() --播放
```