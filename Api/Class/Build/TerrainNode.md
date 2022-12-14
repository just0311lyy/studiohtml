# Terrain
------------------------------------------------------------------------------------------
## 描述

`Terrain`（地形）允许更改或者获取某个位置的方块以及方块实例；

*继承自*：
* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md)

------------------------------------------------------------------------------------------
## 属性

------------------------------------------------------------------------------------------
## 函数

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsAirBlock</font> ](/Api/Class/Build/TerrainNode_F/IsAirBlock.md) ([int](/Api/DataType/Int.md) x, [int](/Api/DataType/Int.md) y, [int](/Api/DataType/Int.md) z)</div>|
|:---|
|位置在（x,y,z）的方块是否是空气方块|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">SetBlockAll</font> ](/Api/Class/Build/TerrainNode_F/SetBlockAll.md) ([int](/Api/DataType/Int.md) x, [int](/Api/DataType/Int.md) y, [int](/Api/DataType/Int.md) z, [int](/Api/DataType/Int.md) blockid, [int](/Api/DataType/Int.md) blockdata)</div>|
|:---|
|设置位置（x,y,z）为XXX方块，并且设置该位置的`blockdata`|

|<div style="width:1000px">[SandboxNode](/Api/Class/NoType/SandboxNode.md) &emsp;[<font color="dd00dd">GetBlockMaterial</font> ](/Api/Class/Build/TerrainNode_F/GetBlockMaterial.md) ([int](/Api/DataType/Int.md) x, [int](/Api/DataType/Int.md) y, [int](/Api/DataType/Int.md) z)</div>|
|:---|
|获取位置（x,y,z）的方块|

|<div style="width:1000px">[SandboxNode](/Api/Class/NoType/SandboxNode.md) &emsp;[<font color="dd00dd">GetBlockNode</font> ](/Api/Class/Build/TerrainNode_F/GetBlockNode.md) ([int](/Api/DataType/Int.md) x, [int](/Api/DataType/Int.md) y, [int](/Api/DataType/Int.md) z)</div>|
|:---|
|获取位置（x,y,z）的方块实例|

------------------------------------------------------------------------------------------
## 示例代码

```lua
local TerrainNode = game.WorkSpace.Terrain
local posx, posy, posz = 0,0,1
local grassid = 100
local blockdata = 0
--在0,0,1位置放置一个草块
TerrainNode:SetBlockAll(posx, posy, posz, grassid, blockdata)
--查询0,0,1位置的方块是不是空气方块，ret:false
local ret = TerrainNode:IsAirBlock(posx, posy, posz)
--获取0,0,1位置的方块
local blockMtl = TerrainNode:GetBlockMaterial(posx, posy, posz)
--pos(0,0,1)is:grass
print("pos(0,0,1)is:"..tostring(blockMtl.Block_Name))
--设置0,0,1位置为楼梯方块
TerrainNode:SetBlockAll(posx, posy, posz, 376, 0)
--获取该位置的方块实例
local blockMtlInstance = TerrainNode:GetBlockNode(posx, posy, posz)
--更改楼梯朝向
blockMtlInstance.BlockData = 2
```