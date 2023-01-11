# PlayersRoot
------------------------------------------------------------------------------------------
## 描述

是一个服务，包含当前已连接到服务器的客户端的所有[`player`](/Api/Class/GamePlay/ScenePlayerObject.md)对象。

*继承自*：
* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md)


------------------------------------------------------------------------------------------
## 属性

|<div style="width:1000px">[SandboxNode](/Api/Class/NoType/SandboxNode.md) &emsp;<font color="dd00dd">LocalPlayer</font></div>|
|:---|
|客户端当前的[`LocalPlayer`](/Api/Class/GamePlay/SandBoxLocalPlayer.md)对象|


|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">MaxPlayers</font>](/Api/Class/GamePlay/SandBoxPlayersRoot_F/1MaxPlayers11.md)</div>|
|:---|
|此服务器中可以容纳的最大玩家数量|

------------------------------------------------------------------------------------------
## 函数

|<div style="width:1000px">[SandboxNode](/Api/Class/NoType/SandboxNode.md) &emsp;[<font color="dd00dd">GetPlayerByUserId</font>](/Api/Class/GamePlay/SandBoxPlayersRoot_F/GetPlayerByUserId.md) ([int](/Api/DataType/Int.md) userId)</div>|
|:---|
|返回给的`serId`的[`player`](/Api/Class/GamePlay/ScenePlayerObject.md)对象|

|<div style="width:1000px">[vector\<SandboxNode\>]() &emsp;[<font color="dd00dd">GetPlayers</font>](/Api/Class/GamePlay/SandBoxPlayersRoot_F/GetPlayers.md) ()</div>|
|:---|
|返回所有目前连接的[`player`](/Api/Class/GamePlay/ScenePlayerObject.md)对象的数组|

------------------------------------------------------------------------------------------
## 事件：

|<div style="width:1125px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;<font color="dd00dd">PlayerConnecting</font></div>|
|:---|
|玩家正在连接游戏时触发|

|<div style="width:1125px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;<font color="dd00dd">PlyerDisconnecting</font></div>|
|:---|
|当玩家正从游戏中断开连接时触发。|

|<div style="width:1125px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;<font color="dd00dd">PlayerRejoining</font></div>|
|:---|
|在玩家断开连接后重新加入游戏会话时触发。|

|<div style="width:500px">[SBXSignal\<SandboxNode\>]() &emsp;<font color="dd00dd">PlayerAdded</font> ()</div>|<div style="width:698px"></div>|
|:---|:---|
|当玩家进入游戏时触发。||
|**返回类型**|**概要**|
|SandboxNode|一个加入游戏的[`player`](/Api/Class/GamePlay/ScenePlayerObject.md)实例|


|<div style="width:500px">[SBXSignal\<SandboxNode\>]() &emsp;<font color="dd00dd">PlayerRemoving</font> ()</div>|<div style="width:698px"></div>|
|:---|:---|
|玩家将要离开游戏时触发。||
|**返回类型**|**概要**|
|SandboxNode|一个离开游戏的[`player`](/Api/Class/GamePlay/ScenePlayerObject.md)实例|


------------------------------------------------------------------------------------------
## 示例代码

```lua
local players = game:GetService("Players")
local playerlist = players:GetPlayers()
for i, v in ipairs( playerlist ) do
    print( v.ClassType )
end
```