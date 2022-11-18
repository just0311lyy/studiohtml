# SandboxCameraObject
------------------------------------------------------------------------------------------
## 描述

对象用于定义`3D`游戏世界的视角。

继承：`SandboxNode` 

------------------------------------------------------------------------------------------
## 属性：

|<div style="width:1125px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">PickPosition</font>](/Api/Class/GamePlay/SandboxCameraObject_F/PickPosition.md)</div>|
|:---|
|摄像机跟随鼠标在游戏内指向的三维坐标(Rainbow::Vector3f)|

|<div style="width:1125px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">LookFocus</font>](/Api/Class/GamePlay/SandboxCameraObject_F/LookFocus.md)</div>|
|:---|
|摄像机焦点，镜头所看向的点|

|<div style="width:1125px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">ZNear</font>](/Api/Class/GamePlay/SandboxCameraObject_F/ZNear.md)</div>|
|:---|
|摄像机的近平面|

|<div style="width:1125px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">ZFar</font>](/Api/Class/GamePlay/SandboxCameraObject_F/ZFar.md)</div>|
|:---|
|摄像机的远平面|

|<div style="width:1125px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">FieldOfView</font>](/Api/Class/GamePlay/SandboxCameraObject_F/FieldOfView.md)</div>|
|:---|
|设置摄像机垂直视野的角度|

|<div style="width:1125px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">CameraType</font>](/Api/Class/GamePlay/SandboxCameraObject_F/CameraType.md)</div>|
|:---|
|摄像机类型|

|<div style="width:1125px">[SandboxNode](/Api/Class/NoType/SandboxNode.md) &emsp;[<font color="dd00dd">CameraSubject</font>](/Api/Class/GamePlay/SandboxCameraObject_F/CameraSubject.md)</div>|
|:---|
|摄像机节点|

|<div style="width:1125px">[Vector2](/Api/DataType/Vector2.md) &emsp;[<font color="dd00dd">ViewportSize</font>](/Api/Class/GamePlay/SandboxCameraObject_F/ViewportSize.md)</div>|
|:---|
|描述客户端视口的尺寸（以像素为单位）(Rainbow::Vector2f)|

|<div style="width:1125px">[Vector2](/Api/DataType/Vector2.md) &emsp;[<font color="dd00dd">WindowSize</font>](/Api/Class/GamePlay/SandboxCameraObject_F/WindowSize.md)</div>|
|:---|
|描述客户端窗口的尺寸（以像素为单位）。<font color="ff3333">（非公开，脚本不可用）</font>|

------------------------------------------------------------------------------------------
## 函数：

|<div style="width:500px">[Ray]() &emsp;[<font color="dd00dd">ViewportPointToRay</font> ](/Api/Class/GamePlay/SandboxCameraObject_F/ViewportPointToRay.md) ( [float](/Api/DataType/Float.md) x , [float](/Api/DataType/Float.md ) y , [float](/Api/DataType/Float.md) depth=0)</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|以朝向摄像机的方向，通过给定的距摄像机的深度，<br>在视口上的某个位置创建单位射线（以像素为单位）||||
|**参数名称**|**类别**|**默认**|**描述**|
|x|float||x坐标|
|y|float||y坐标|
|depth|float||深度|
|**返回类型**|||**概要**|
|Ray|||射线|

|<div style="width:500px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">WorldToViewportPoint</font> ](/Api/Class/GamePlay/SandboxCameraObject_F/WorldToViewportPoint.md) ( [Vector3](/Api/DataType/Vector3.md) position )</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|将一个世界坐标position转换到摄像机视口坐标||||
|**参数名称**|**类别**|**默认**|**描述**|
|position|Vector3||三维坐标|
|**返回类型**|||**概要**|
|Vector3|||三维坐标|

|<div style="width:500px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">WorldToUIPoint</font> ](/Api/Class/GamePlay/SandboxCameraObject_F/WorldToUIPoint.md) ( [Vector3](/Api/DataType/Vector3.md) position )</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|将3D节点世界坐标position转UI节点坐标||||
|**参数名称**|**类别**|**默认**|**描述**|
|position|Vector3||三维坐标|
|**返回类型**|||**概要**|
|Vector3|||三维坐标|

------------------------------------------------------------------------------------------
## 示例代码

```lua
--创建相机
local camera = SandboxNode.new('SandboxCameraObject')
local workSpace = game.WorkSpace
--设置父节点
camera:SetParent(workSpace)
--设置视角大小
camera.FieldOfView = 100.0
--设置相机位置
camera.Position = Vector3.new(500, 700, 500)
```