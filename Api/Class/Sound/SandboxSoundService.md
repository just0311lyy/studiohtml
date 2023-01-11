# SoundService
------------------------------------------------------------------------------------------
## 描述

此类是一个服务！它是顶级单例，可以使用`GetService`函数获取。为负责将 `Players`玩家在不同服务器和场景间进行传送的服务。

*继承自*：
* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md)

------------------------------------------------------------------------------------------
## 属性

|<div style="width:1000px">[EnumListenerType](/Api/Enumerate/Sound/EnumListenerType.md)  &emsp;<font color="dd00dd">ListenerType</font> </div>|
|:---|
|设置当前监听类型，具体参考：[EnumListenerType](/Api/Enumerate/Sound/EnumListenerType.md)<br>	只可在脚本获取，不可写。 |

|<div style="width:1000px">[SandboxNode](/Api/Class/NoType/SandboxNode.md)  &emsp;<font color="dd00dd">ListenerObject</font> </div>|
|:---|
|只可在脚本获取，不可写，当[`ListenerType`](/Api/Enumerate/Sound/EnumListenerType.md)为`Camrea`时返回`nil`，当[`ListenerType`](/Api/Enumerate/Sound/EnumListenerType.md)为`TransObject`时,返回`TransObject`节点指针|

|<div style="width:1000px">[float](/Api/DataType/Float.md)  &emsp;<font color="dd00dd">RolloffScale</font> </div>|
|:---|
|3D声音衰减速度|

|<div style="width:1000px">[float](/Api/DataType/Float.md)  &emsp;<font color="dd00dd">DistanceFactor</font> </div>|
|:---|
|3D声音衰减距离|

|<div style="width:1000px">[float](/Api/DataType/Float.md)   &emsp;<font color="dd00dd">DopplerScale</font> </div>|
|:---|
|3D声音多普勒效应强度|


------------------------------------------------------------------------------------------
## 函数

|<div style="width:1000px">[void](/Api/Parameter/void.md)  &emsp;[<font color="dd00dd">SetListener</font> ](/Api/Class/Sound/SandboxSoundService_F/SetListener.md)( [EnumListenerType](/Api/Enumerate/Sound/EnumListenerType.md) type, [SandboxNode](/Api/Class/NoType/SandboxNode.md) object )</div>
|:---|
|设置监听类型与监听者|

|<div style="width:1000px">[void](/Api/Parameter/void.md)  &emsp;[<font color="dd00dd">PlayerLocalSound</font> ](/Api/Class/Sound/SandboxSoundService_F/PlayerLocalSound.md)( [SandboxNode](/Api/Class/NoType/SandboxNode.md) sound )</div>|
|:---|
|在本地播放声音节点（2D，不会同步）|

|<div style="width:1000px">[void](/Api/Parameter/void.md)  &emsp;[<font color="dd00dd">SetSoundOpen</font> ](/Api/Class/Sound/SandboxSoundService_F/SetSoundOpen.md)([bool](/Api/DataType/Bool.md) value)</div>|
|:---|
|在本地开关声音（包括游戏本身的音乐和声音节点）|

------------------------------------------------------------------------------------------
## 事件


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
