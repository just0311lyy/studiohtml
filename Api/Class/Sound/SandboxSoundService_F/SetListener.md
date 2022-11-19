# SoundType
-----------------------------------------------------------------------------------------
## 描述

函数所属类：[SandboxSoundService](/Api/Class/Sound/SandboxSoundService.md)

设置监听类型与监听者

-----------------------------------------------------------------------------------------
## 参数


|<div style="width:200px">名称</div>|<div style="width:200px">类型</div>|<div style="width:200px">默认</div>|<div style="width:200px">描述</div>|
|:--------------------|:--------------------|:--------------------|:--------------------|
|type|[EnumListenerType](/Api/Enumerate/Sound/EnumListenerType.md)||[EnumListenerType](/Api/Enumerate/Sound/EnumListenerType.md)|
|object|[SandBoxNode](/Api/Class/NoType/SandBoxNode.md)||监听者|

## 返回

无返回值

------------------------------------------------------------------------------------------
## 示例代码：

```lua
local SoundService = game:GetService("SoundService")
SoundService:SetSoundOpen(true)                    --打开声音
local listenertype = SoundService.ListenerType     --监听类型
local listenerobject = SoundService.ListenerObject --监听对象
SoundService.RolloffScale = 1                      --衰减速度
SoundService.DistanceFactor = 0                    --衰减距离
SoundService.DopplerScale = 0                      --多普勒效应强度
local soundnode = game.WorkSpace.Sound             --获取Sound节点
SoundService:PlayerLocalSound(soundnode)           --本地播放
local transnode = game.WorkSpace.TransNode         --获取TransObject节点
SoundService:SetListener(Enum.EnumListenerType.TransObject,transnode)       --设置监听者
```