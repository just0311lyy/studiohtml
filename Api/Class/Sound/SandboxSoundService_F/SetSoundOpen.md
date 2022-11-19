# SetSoundOpen
-----------------------------------------------------------------------------------------
## 描述

函数所属类：[SandboxSoundService](/Api/Class/Sound/SandboxSoundService.md)

在本地开关声音（包括游戏本身的音乐和声音节点）

-----------------------------------------------------------------------------------------
## 参数


|<div style="width:200px">名称</div>|<div style="width:200px">类型</div>|<div style="width:200px">默认</div>|<div style="width:200px">描述</div>|
|:--------------------|:--------------------|:--------------------|:--------------------|
|value|[bool](/Api/DataType/Bool.md)||声音开关，为`true`，开启声音|

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