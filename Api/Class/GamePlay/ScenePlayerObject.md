# Player
------------------------------------------------------------------------------------------
## 描述：

*继承自*：
* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md)

------------------------------------------------------------------------------------------
## 属性：

|<div style="width:1000px">[SandboxNode](/Api/Class/NoType/SandboxNode.md) &emsp;<font color="dd00dd">Character</font></div>|
|:---|
|行为|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Neutral</font></div>|
|:---|
|是否中立|

|<div style="width:1000px">[SandboxNode](/Api/Class/NoType/SandboxNode.md) &emsp;<font color="dd00dd">Team</font></div>|
|:---|
|隶属Team|

|<div style="width:1000px">[ColorValue](/Api/DataType/colorValue.md) &emsp;<font color="dd00dd">TeamColor</font></div>|
|:---|
|隶属Team的颜色值|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;<font color="dd00dd">UserId</font></div>|
|:---|
|用户UserId|

|<div style="width:1000px">[SandboxNode](/Api/Class/NoType/SandboxNode.md) &emsp;<font color="dd00dd">Backpack</font></div>|
|:---|
|背包|

|<div style="width:1000px">[SandboxNode](/Api/Class/NoType/SandboxNode.md) &emsp;<font color="dd00dd">ActorObject</font></div>|
|:---|
|生物对象|

|<div style="width:1000px">[CameraMode]() &emsp;<font color="dd00dd">CameraMode</font></div>|
|:---|
|相机模式（第一人称或第三人称视角）|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;<font color="dd00dd">CameraMaxZoomDistance</font></div>|
|:---|
|玩家镜头的最大拉远距离|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;<font color="dd00dd">CameraMinZoomDistance</font></div>|
|:---|
|玩家镜头的最大拉近距离|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;<font color="dd00dd">nameDisplayDistance</font></div>|
|:---|
|设置其他 Humanoid 名称对当前玩家的可见距离。设置为 0 时将隐藏所有名称|

------------------------------------------------------------------------------------------
## 函数：

|<div style="width:1000px">[SandboxNode](/Api/Class/NoType/SandboxNode.md) &emsp;[<font color="dd00dd">WaitForChild</font>](/Api/Class/GamePlay/ScenePlayerObject_F/WaitForChild.md) ([string](/Api/DataType/String.md) child)</div>|
|:---|
|通过名获取沙盒子节点|

|<div style="width:1000px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">EyePos</font>](/Api/Class/GamePlay/ScenePlayerObject_F/EyePos.md) ([Vector3](/Api/DataType/Vector3.md) pos, [Vector3](/Api/DataType/Vector3.md) dir, [float](/Api/DataType/Float.md) dist)</div>|
|:---|
|校准碰撞视线位置（仅脚本可用）|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">EquipTool</font>](/Api/Class/GamePlay/ScenePlayerObject_F/EquipTool.md) ([SandboxNode](/Api/Class/NoType/SandboxNode.md) tool)</div>|
|:---|
|给[`player`](/Api/Class/GamePlay/ScenePlayerObject.md)装备上指定的[`tool`](/Api/Class/GamePlay/SandboxTool.md)|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;<font color="dd00dd">UnequipTools</font>( )</div>|
|:---|
|解除[`player`](/Api/Class/GamePlay/ScenePlayerObject.md)的装备|

------------------------------------------------------------------------------------------
## 事件：

|<div style="width:500px">[SBXSignal\<float\>]() &emsp;<font color="dd00dd">Idle</font> ( )</div>|<div style="width:698px"></div>|
|:---|:---|
|通常在游戏引擎将玩家定类为闲置状态的两分钟后进行触发。`Time`（时间）为此时点后所经历的秒数||
|**返回类型**|**概要**|
|float|限制状态触发时间|

