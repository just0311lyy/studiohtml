# Backpack

------------------------------------------------------------------------------------------
## 描述

存放`ScenePlayerObject`物品栏的容器对象。玩家[`Backpack`](/Api/Class/GamePlay/SandboxBackpack.md)中的所有`SandboxTool`都会显示在他们屏幕下方的物品栏中。从物品栏中选择`SandboxTool`会装备`SandboxTool`，将其从[`Backpack`](/Api/Class/GamePlay/SandboxBackpack.md)中转移到玩家角色上。

*继承自*：
* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md)

------------------------------------------------------------------------------------------
## 属性

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CoreUiEnabled</font></div>|
|:---|
|是否显示默认的快捷栏`UI`，默认值为`false`|

------------------------------------------------------------------------------------------
## 函数

|<div style="width:1000px">[SandboxNode](/Api/Class/NoType/SandboxNode.md) &emsp;[<font color="dd00dd">GetTool</font> ](/Api/Class/GamePlay/SandboxBackpack_F/GetTool.md) ([int](/Api/DataType/Int.md) index)</div>|
|:---|
|获取某个键位对应的[`tool`](/Api/Class/GamePlay/SandboxTool.md)，`index`从1开始|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetTool</font> ](/Api/Class/GamePlay/SandboxBackpack_F/SetTool.md) ([int](/Api/DataType/Int.md) index, [SandboxNode](/Api/Class/NoType/SandboxNode.md) tool)</div>|
|:---|
|设置[`tool`](/Api/Class/GamePlay/SandboxTool.md)到具体的快捷键位置|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">RemoveTool</font> ](/Api/Class/GamePlay/SandboxBackpack_F/RemoveTool.md) ([int](/Api/DataType/Int.md) index)</div>|
|:---|
|移除tool|

------------------------------------------------------------------------------------------
## 事件

|<div style="width:1000px">[SBXSignal\<int\>]() &emsp;<font color="dd00dd">GetCurEquipedTool</font>  ()</div>|<div style="width:698px"></div>|
|:---|:---|
|获取当前装备的[`tool`](/Api/Class/GamePlay/SandboxTool.md)||
|**返回类型**|**概要**|
|SandboxNode|当前装备的[`tool`](/Api/Class/GamePlay/SandboxTool.md)|

