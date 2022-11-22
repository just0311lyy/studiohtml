# SandboxTeam
------------------------------------------------------------------------------------------
## 描述

沙盒游戏场景中的队伍或派系。`Team`的唯一有效父项为`Teams`服务内。

继承：`SandboxNode` 

------------------------------------------------------------------------------------------
## 属性

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">AutoAssignable</font>](/Api/Class/GamePlay/SandboxTeam_F/AutoAssignable.md)</div>|
|:---|
|此属性用来决定加入游戏的`Player`是否允许自动分配到该队伍|

|<div style="width:1000px">[ColorValue](/Api/DataType/ColourValue.md) &emsp;[<font color="dd00dd">TeamColor</font>](/Api/Class/GamePlay/SandboxTeam_F/TeamColor.md)</div>|
|:---|
|此属性设置`Team`的颜色，决定队伍成员的`Player.TeamColor`属性   (`Rainbow::ColorQuad`)|

------------------------------------------------------------------------------------------
## 函数

------------------------------------------------------------------------------------------
## 事件
|<div style="width:500px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;[<font color="dd00dd">PlayerAdded</font> ](/Api/Class/GamePlay/SandboxTeam_F/PlayerAdded.md) ( [SandboxNode](/Api/Class/NoType/SandboxNode.md) )</div>|<div style="width:698px"></div>|
|:---|:---|
|新增一个玩家||
|**返回类型**|**概要**|
|SandboxNode|玩家节点对象|

|<div style="width:500px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;[<font color="dd00dd">PlayerRemoved</font> ](/Api/Class/GamePlay/SandboxTeam_F/SendChatText.md) ( [SandboxNode](/Api/Class/NoType/SandboxNode.md) )</div>|<div style="width:698px"></div>|
|:---|:---|
|移除一个玩家||
|**返回类型**|**概要**|
|SandboxNode|玩家节点对象|

------------------------------------------------------------------------------------------
## 示例代码

```lua
local Teams = game:GetService('Teams')
--创建开始队伍
local team1 = SandboxNode.new('SandboxTeam', Teams)
team1.AutoAssignable = true
Teams.TeamColor = Vector3.new(255, 0, 0)
```