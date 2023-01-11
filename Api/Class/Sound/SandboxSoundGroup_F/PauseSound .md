# ChangeVolume
-----------------------------------------------------------------------------------------
## 描述

函数所属类：[SandboxSoundGroup](/Api/Class/Sound/SandboxSoundGroup.md)

按比例改变组内声音音量（0~1），如：传入0.5会将组内[`Sound`](/Api/Class/Sound/SandboxSound.md)节点音量减半

-----------------------------------------------------------------------------------------
## 参数


|<div style="width:200px">名称</div>|<div style="width:200px">类型</div>|<div style="width:200px">默认</div>|<div style="width:200px">描述</div>|
|:--------------------|:--------------------|:--------------------|:--------------------|
|vaval|float||置组内声音音量（0~1），0.5音量减半|


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