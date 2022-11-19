# ScenePlayerObject
------------------------------------------------------------------------------------------
## 描述：

继承：`SandboxNode` 

------------------------------------------------------------------------------------------
## 属性：

|<div style="width:1125px">[SandboxNode](/Api/Class/NoType/SandboxNode.md) &emsp;[<font color="dd00dd">Character</font>](/Api/Class/GamePlay/ScenePlayerObject_F/Character.md)</div>|
|:---|
|行为|

|<div style="width:1125px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">Neutral</font>](/Api/Class/GamePlay/ScenePlayerObject_F/Neutral.md)</div>|
|:---|
|是否中立|

|<div style="width:1125px">[SandboxNode](/Api/Class/NoType/SandboxNode.md) &emsp;[<font color="dd00dd">Team</font>](/Api/Class/GamePlay/ScenePlayerObject_F/Team.md)</div>|
|:---|
|隶属Team|

|<div style="width:1125px">[ColorValue](/Api/DataType/ColourValue.md) &emsp;[<font color="dd00dd">TeamColor</font>](/Api/Class/GamePlay/ScenePlayerObject_F/TeamColor.md)</div>|
|:---|
|隶属Team的颜色值|

|<div style="width:1125px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">UserId</font>](/Api/Class/GamePlay/ScenePlayerObject_F/UserId.md)</div>|
|:---|
|用户UserId|

|<div style="width:1125px">[SandboxNode](/Api/Class/NoType/SandboxNode.md) &emsp;[<font color="dd00dd">Backpack</font>](/Api/Class/GamePlay/ScenePlayerObject_F/Backpack.md)</div>|
|:---|
|背包|

|<div style="width:1125px">[SandboxNode](/Api/Class/NoType/SandboxNode.md) &emsp;[<font color="dd00dd">ActorObject</font>](/Api/Class/GamePlay/ScenePlayerObject_F/ActorObject.md)</div>|
|:---|
|生物对象|

|<div style="width:1125px">[CameraMode]() &emsp;[<font color="dd00dd">CameraMode</font>](/Api/Class/GamePlay/ScenePlayerObject_F/CameraMode.md)</div>|
|:---|
|相机模式（第一人称或第三人称视角）|

|<div style="width:1125px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">CameraMaxZoomDistance</font>](/Api/Class/GamePlay/ScenePlayerObject_F/CameraMaxZoomDistance.md)</div>|
|:---|
|玩家镜头的最大拉远距离|

|<div style="width:1125px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">CameraMinZoomDistance</font>](/Api/Class/GamePlay/ScenePlayerObject_F/CameraMinZoomDistance.md)</div>|
|:---|
|玩家镜头的最大拉近距离|

|<div style="width:1125px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">nameDisplayDistance</font>](/Api/Class/GamePlay/ScenePlayerObject_F/nameDisplayDistance.md)</div>|
|:---|
|设置其他 Humanoid 名称对当前玩家的可见距离。设置为 0 时将隐藏所有名称|

------------------------------------------------------------------------------------------
## 函数：

|<div style="width:500px">[SandboxNode](/Api/Class/NoType/SandboxNode.md) &emsp;[<font color="dd00dd">WaitForChild</font>](/Api/Class/GamePlay/ScenePlayerObject_F/WaitForChild.md) ([string](/Api/DataType/String.md) child)</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|通过名获取沙盒子节点||||
|**参数名称**|**类别**|**默认**|**描述**|
|child|string||节点name名|
|**返回类型**|||**概要**|
|SandboxNode|||沙盒子节点|

|<div style="width:500px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">EyePos</font>](/Api/Class/GamePlay/ScenePlayerObject_F/EyePos.md) ([Vector3](/Api/DataType/Vector3.md) pos, [Vector3](/Api/DataType/Vector3.md) dir, [float](/Api/DataType/Float.md) dist)</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|校准碰撞视线位置（仅脚本可用）||||
|**参数名称**|**类别**|**默认**|**描述**|
|pos|Vector3||世界坐标|
|dir|Vector3||朝向|
|dist|Vector3||射线途径的距离长度|
|**返回类型**|||**概要**|
|Vector3|||世界坐标|

|<div style="width:500px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">EquipTool</font>](/Api/Class/GamePlay/ScenePlayerObject_F/EquipTool.md) ([SandboxNode](/Api/Class/NoType/SandboxNode.md) tool)</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|给`player`装备上指定的`tool`||||
|**参数名称**|**类别**|**默认**|**描述**|
|tool|SandboxNode||即将装备的Tool|

|<div style="width:1125px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">UnequipTools</font>](/Api/Class/GamePlay/ScenePlayerObject_F/UnequipTools.md)( )</div>|
|:---|
|解除`player`的装备|

------------------------------------------------------------------------------------------
## 事件：

|<div style="width:500px">[SBXSignal\<float\>]() &emsp;[<font color="dd00dd">Idle</font>](/Api/Class/GamePlay/ScenePlayerObject_F/Idle.md) ( )</div>|<div style="width:698px"></div>|
|:---|:---|
|通常在游戏引擎将玩家定类为闲置状态的两分钟后进行触发。`Time`（时间）为此时点后所经历的秒数||
|**返回类型**|**概要**|
|float|限制状态触发时间|
