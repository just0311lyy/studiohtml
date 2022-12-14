# TeleportService
------------------------------------------------------------------------------------------
## 描述

此类是一个服务！它是顶级单例，可以使用`GetService`函数获取。为负责将 `Players`玩家在不同服务器和场景间进行传送的服务。

*继承自*：
* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md)

------------------------------------------------------------------------------------------
## 属性

------------------------------------------------------------------------------------------
## 函数

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">teleport</font> ](/Api/Class/GamePlay/SandboxTeleportService_F/teleport.md) ([SandboxNode](/Api/Class/NoType/SandboxNode.md) playernode, [Vector3](/Api/DataType/Vector3.md) pos)</div>|
|:---|
|地图内将玩家传送到指定位置|


------------------------------------------------------------------------------------------
## 事件

|<div style="width:1000px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;[<font color="dd00dd">TeleportSuccess</font>](/Api/Class/GamePlay/SandboxTeleportService_F/TeleportSuccess.md)( )</div>|
|:---|
|玩家传送成功触发|

|<div style="width:1000px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;[<font color="dd00dd">TeleportFail</font>](/Api/Class/GamePlay/SandboxTeleportService_F/TeleportFail.md)( )</div>|
|:---|
|玩家传送失败触发|

------------------------------------------------------------------------------------------
## 示例代码

```lua
local TeleportService= game:GetService('TeleportService')
TeleportService:teleport(player, Vector3.new(500, 700, 800))
```