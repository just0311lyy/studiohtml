# SpawnLocation
------------------------------------------------------------------------------------------
## 描述

可确定[`Player`](/Api/Class/GamePlay/ScenePlayerObject.md)（玩家）死亡时在何处重生

*继承自*：
* [ScenePrimitiveObject](/Api/Class/Bind/ScenePrimitiveObject.md)

------------------------------------------------------------------------------------------
## 属性

|<div style="width:1125px">[bool](/Api/DataType/Bool.md)&emsp;<font color="dd00dd">Neutral</font></div>|
|:---|
|是否隶属与特定队伍，设置为`true`之后，任意队伍中的任意[`Player`](/Api/Class/GamePlay/ScenePlayerObject.md)可以在此位置重生|


|<div style="width:1125px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">AllowTeamChangeOnTouch</font></div>|
|:---|
|是否允许[`Player`](/Api/Class/GamePlay/ScenePlayerObject.md)通过`Touch`触摸该`Location`来加入对应`TeamColor`的[`Team`](/Api/Class/GamePlay/SandboxTeam.md)队伍|

|<div style="width:1125px">[ColorQuad](/Api/DataType/ColorQuad.md) &emsp;<font color="dd00dd">TeamColor</font></div>|
|:---|
|队伍颜色(`Rainbow::ColorQuad`)，跟`TeamColor`可对应|

------------------------------------------------------------------------------------------
## 函数

------------------------------------------------------------------------------------------
## 示例代码

```lua
local Teams = game:GetService('Teams')
--创建开始队伍
local team1 = SandboxNode.new('SandboxTeam', Teams)
team1.AutoAssignable = true
team1.TeamColor = Vector3.new(255, 0, 0)

--创建重生点
local team1Spawn = SandboxNode.new('SpawnLocation', game.WorkSpace)
team1Spawn.Neutral = false
team1Spawn.AllowTeamChangeOnTouch = true
team1Spawn.TeamColor = team1.TeamColor
```