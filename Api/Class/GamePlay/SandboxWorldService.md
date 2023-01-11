# WorldService
------------------------------------------------------------------------------------------
## 描述

此类是一个服务！它是顶级单例，可以使用`GetService`函数获取。<br>
提供跟`chunk`、`world`交互的功能性接口。

*继承自*：
* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md)

------------------------------------------------------------------------------------------
## 属性：

------------------------------------------------------------------------------------------
## 函数：

|<div style="width:1000px">[ReflexTuple](/Api/Parameter/Tuple.md) &emsp;[<font color="dd00dd">GetRangeXZ</font> ](/Api/Class/GamePlay/SandboxWorldService_F/GetRangeXZ.md) ()</div>|
|:---|
|获取当前所在`chunk`的首尾 xz 的坐标|



|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">GetRayBlock</font> ](/Api/Class/GamePlay/SandboxWorldService_F/GetRayBlock.md) ([Vector3](/Api/DataType/Vector3.md) vector3 ,  [int](/Api/DataType/Int.md) face ,  [float](/Api/DataType/Float.md) distance)</div>|
|:---|
|获取射线碰撞到的方块id|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsSolidBlock</font> ](/Api/Class/GamePlay/SandboxWorldService_F/IsSolidBlock.md) ([Vector3](/Api/DataType/Vector3.md) vector3)</div>|
|:---|
|判断该位置是否是刚体方块|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsLiquidBlock</font> ](/Api/Class/GamePlay/SandboxWorldService_F/IsLiquidBlock.md) ([Vector3](/Api/DataType/Vector3.md) vector3)</div>|
|:---|
|判断该位置是否是流体方块|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsAirBlock</font> ](/Api/Class/GamePlay/SandboxWorldService_F/IsAirBlock.md) ([Vector3](/Api/DataType/Vector3.md) vector3)</div>|
|:---|
|判断该位置是否是空气方块|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">GetBlockData</font> ](/Api/Class/GamePlay/SandboxWorldService_F/GetBlockData.md) ([Vector3](/Api/DataType/Vector3.md) vector3)</div>|
|:---|
|获取该位置方块的`blockdata`数据|

|<div style="width:1000px">[Vector2](/Api/DataType/Vector2.md) &emsp;[<font color="dd00dd">GetUIScale</font> ](/Api/Class/GamePlay/SandboxWorldService_F/GetUIScale.md) ()</div>|
|:---|
|获取UI布局的缩放大小|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetBlock</font> ](/Api/Class/GamePlay/SandboxWorldService_F/SetBlock.md) ([Vector3](/Api/DataType/Vector3.md) pos , [int](/Api/DataType/Int.md) blockid , [int](/Api/DataType/Int.md) data , [int](/Api/DataType/Int.md) flags , [bool](/Api/DataType/Bool.md) forceupdate)</div>|
|:---|
|放置方块|

|<div style="width:1000px">ReflexMap &emsp;[<font color="dd00dd">RaycastClosest</font> ](/Api/Class/GamePlay/SandboxWorldService_F/RaycastClosest.md) ([Vector3](/Api/DataType/Vector3.md) origin ,  [Vector3](/Api/DataType/Vector3.md) unitDir ,  [float](/Api/DataType/Float.md) distance ,  [bool](/Api/DataType/Bool.md) isIgnoreTrigger ,  [int](/Api/DataType/Int.md) filterGroup)</div>|
|:---|
|射线段检测，返回最近的碰撞物|


|<div style="width:1000px">[vector\<ReflexMap\>]() &emsp;[<font color="dd00dd">RaycastAll</font> ](/Api/Class/GamePlay/SandboxWorldService_F/RaycastAll.md) ([Vector3](/Api/DataType/Vector3.md) origin ,  [Vector3](/Api/DataType/Vector3.md) unitDir ,  [float](/Api/DataType/Float.md) distance ,  [bool](/Api/DataType/Bool.md) isIgnoreTrigger ,  [int](/Api/DataType/Int.md) filterGroup)</div>|
|:---|
|射线段检测，返回所有碰撞物，最多128个|

|<div style="width:1000px">[SandboxNode](/Api/Class/NoType/SandboxNode.md) &emsp;[<font color="dd00dd">GetBlockNode</font> ](/Api/Class/GamePlay/SandboxWorldService_F/GetBlockNode.md) ([Vector3](/Api/DataType/Vector3.md) pos)</div>|
|:---|
|获取方块节点|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">DropBlockAsItem</font> ](/Api/Class/GamePlay/SandboxWorldService_F/DropBlockAsItem.md) ([Vector3](/Api/DataType/Vector3.md) pos ,  [int](/Api/DataType/Int.md) droptype ,  [float](/Api/DataType/Float.md) chance ,  [int](/Api/DataType/Int.md) useToolId)</div>|
|:---|
|方块掉落道具|

|<div style="width:1000px">ReflexMap &emsp;[<font color="dd00dd">SweepBox</font> ](/Api/Class/GamePlay/SandboxWorldService_F/SweepBox.md) ([Vector3](/Api/DataType/Vector3.md) center ,  [Vector3](/Api/DataType/Vector3.md) shape ,  [Vector3](/Api/DataType/Vector3.md) direction ,  [Vector3](/Api/DataType/Vector3.md) angle ,  [float](/Api/DataType/Float.md) distance ,  [bool](/Api/DataType/Bool.md) isIgnoreTrigger ,  [int](/Api/DataType/Int.md) filterGroup)</div>|
|:---|
|扫描框|

|<div style="width:1000px">[vector\<ReflexMap\>]() &emsp;[<font color="dd00dd">SweepBoxAll</font> ](/Api/Class/GamePlay/SandboxWorldService_F/SweepBoxAll.md) ([Vector3](/Api/DataType/Vector3.md) center ,  [Vector3](/Api/DataType/Vector3.md) shape ,  [Vector3](/Api/DataType/Vector3.md) direction ,  [Vector3](/Api/DataType/Vector3.md) angle ,  [float](/Api/DataType/Float.md) distance ,  [bool](/Api/DataType/Bool.md) isIgnoreTrigger ,  [int](/Api/DataType/Int.md)</div>|
|:---|
|扫描框全部|

|<div style="width:1000px">ReflexMap &emsp;[<font color="dd00dd">SweepCapsule</font> ](/Api/Class/GamePlay/SandboxWorldService_F/SweepCapsule.md) ([float](/Api/DataType/Float.md) radius ,  [Vector3](/Api/DataType/Vector3.md) p0 ,  [Vector3](/Api/DataType/Vector3.md) p1 ,  [Vector3](/Api/DataType/Vector3.md) dir ,  [float](/Api/DataType/Float.md) distance ,  [bool](/Api/DataType/Bool.md) isIgnoreTrigger ,  [int](/Api/DataType/Int.md) filterGroup)</div>|
|:---|
|扫描胶囊|

|<div style="width:1000px">[vector\<ReflexMap\>]() &emsp;[<font color="dd00dd">SweepCapsuleAll</font> ](/Api/Class/GamePlay/SandboxWorldService_F/SweepCapsuleAll.md) ([float](/Api/DataType/Float.md) radius ,  [Vector3](/Api/DataType/Vector3.md) p0 ,  [Vector3](/Api/DataType/Vector3.md) p1 ,  [Vector3](/Api/DataType/Vector3.md) dir ,  [float](/Api/DataType/Float.md) distance ,  [bool](/Api/DataType/Bool.md) isIgnoreTrigger ,  [int](/Api/DataType/Int.md) filterGroup]() filterGroup)</div>|
|:---|
|扫描胶囊全部|

|<div style="width:1000px">ReflexMap &emsp;[<font color="dd00dd">SweepSphere</font> ](/Api/Class/GamePlay/SandboxWorldService_F/SweepSphere.md) ([float](/Api/DataType/Float.md) radius ,  [Vector3](/Api/DataType/Vector3.md) center ,  [Vector3](/Api/DataType/Vector3.md) direction ,  [float](/Api/DataType/Float.md) distance ,  [bool](/Api/DataType/Bool.md) isIgnoreTrigger ,  [int](/Api/DataType/Int.md) filterGroup)</div>|
|:---|
|扫描球体|

|<div style="width:1000px">[vector\<ReflexMap\>]() &emsp;[<font color="dd00dd">SweepSphereAll</font> ](/Api/Class/GamePlay/SandboxWorldService_F/SweepSphereAll.md) ([float](/Api/DataType/Float.md) radius ,  [Vector3](/Api/DataType/Vector3.md) center ,  [Vector3](/Api/DataType/Vector3.md) direction ,  [float](/Api/DataType/Float.md) distance ,  [bool](/Api/DataType/Bool.md) isIgnoreTrigger ,  [int](/Api/DataType/Int.md) filterGroup)</div>|
|:---|
|扫描球全部|

|<div style="width:1000px">[vector\<ReflexMap\>]() &emsp;[<font color="dd00dd">OverlapBox</font> ](/Api/Class/GamePlay/SandboxWorldService_F/OverlapBox.md) ([Vector3](/Api/DataType/Vector3.md) shape ,  [Vector3](/Api/DataType/Vector3.md) pos ,  [Vector3](/Api/DataType/Vector3.md) angle ,  [bool](/Api/DataType/Bool.md) isIgnoreTrigger ,  [int](/Api/DataType/Int.md) filterGroup)</div>|
|:---|
|重叠框|

|<div style="width:1000px">[vector\<ReflexMap\>]() &emsp;[<font color="dd00dd">OverlapCapsule</font> ](/Api/Class/GamePlay/SandboxWorldService_F/OverlapCapsule.md) ([float](/Api/DataType/Float.md) radius ,  [Vector3](/Api/DataType/Vector3.md) p0 ,  [Vector3](/Api/DataType/Vector3.md) p1 ,  [bool](/Api/DataType/Bool.md) isIgnoreTrigger ,  [int](/Api/DataType/Int.md) filterGroup)</div>|
|:---|
|重叠胶囊|

|<div style="width:1000px">[vector\<ReflexMap\>]() &emsp;[<font color="dd00dd">OverlapSphere</font> ](/Api/Class/GamePlay/SandboxWorldService_F/OverlapSphere.md) ([float](/Api/DataType/Float.md) radius ,  [Vector3](/Api/DataType/Vector3.md) pos ,  [bool](/Api/DataType/Bool.md) isIgnoreTrigger ,  [int](/Api/DataType/Int.md) filterGroup)</div>|
|:---|
|重叠球体|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetMainFrameShow</font> ](/Api/Class/GamePlay/SandboxWorldService_F/SetMainFrameShow.md) ([bool](/Api/DataType/Bool.md) isShow)</div>|
|:---|
|锁定时间|

|<div style="width:500px">[Vector2](/Api/DataType/Vector2.md) &emsp;[<font color="dd00dd">GetUISize</font> ](/Api/Class/GamePlay/SandboxWorldService_F/GetUISize.md) ()</div>|
|:---|
|获取UI布局的尺寸|


------------------------------------------------------------------------------------------
## 示例代码：
```lua
local worldService = game:GetService('WorldService')
local ret = worldService:IsAirBlock(Vector3.new(500, 700, 800))
print("the pos block is airBlock = ", ret)
```