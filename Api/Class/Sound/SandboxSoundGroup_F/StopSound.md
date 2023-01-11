# PlaySound
-----------------------------------------------------------------------------------------
## 描述

函数所属类：[SandboxSoundGroup](/Api/Class/Sound/SandboxSoundGroup.md)

停止播放，会暂停声音组内所有声音

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