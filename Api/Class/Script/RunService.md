# RunService
-----------------------------------------------------------------------------------------
## 描述

此类是一个服务！它是顶级单例，可以使用[`GetService`]()函数获取。包含了用于时间管理的方法和事件，以及管理游戏或脚本所处于的内容。IsClient、IsServer、IsStudio 等方法可以帮助你确定 Lua 代码在哪里运行。这些方法对于客户端和服务器都需要的 ModuleScript 是很有帮助的。

继承自：
* [`ServiceNode `]()

------------------------------------------------------------------------------------------
## 属性


------------------------------------------------------------------------------------------
## 函数


|<div style="width:925px">[bool](/Api/DataType/Bool.md)&emsp; [<font color="dd00dd">IsClient</font>](/Api/Class/Script/RunService_F/IsClient.md)(&nbsp;)</div>|
|:---|
|返回当前的环境是否运行在客户端上。（`true`, 运行在客户端上; `false`, 运行在服务端上）|



|<div style="width:925px">[bool](/Api/DataType/Bool.md)&emsp; [<font color="dd00dd">IsServer</font>](/Api/Class/Script/RunService_F/IsServer.md)(&nbsp;)</div>|
|:---|
|返回当前的环境是否运行在服务器上|


|<div style="width:925px">[bool](/Api/DataType/Bool.md)&emsp; [<font color="dd00dd">IsRemote</font>](/Api/Class/Script/RunService_F/IsRemote.md)(&nbsp;)</div>|
|:---|
|返回当前的环境是否远程|

|<div style="width:925px">[bool](/Api/DataType/Bool.md)&emsp; [<font color="dd00dd">IsEdit</font>](/Api/Class/Script/RunService_F/IsEdit.md)(&nbsp;)</div>|
|:---|
|返回当前运行环境是否为`Edit`（编辑)模式|

|<div style="width:925px">[bool](/Api/DataType/Bool.md)&emsp; [<font color="dd00dd">IsRunMode</font>](/Api/Class/Script/RunService_F/IsRunMode.md)(&nbsp;)</div>|
|:---|
|返回当前运行环境是否为`Running`模式|

|<div style="width:925px">[bool](/Api/DataType/Bool.md)&emsp; [<font color="dd00dd">Pause</font>](/Api/Class/Script/RunService_F/Pause.md)(&nbsp;)</div>|
|:---|
|如果游戏在运行则暂停游戏的模拟，暂停物理运算和脚本|

|<div style="width:925px">[void](/Api/DataType/Nil.md)&emsp; [<font color="dd00dd">BindToRenderStep</font>](/Api/Class/Script/RunService_F/BindToRenderStep.md)(&nbsp;[string](/Api/DataType/String.md) name ，[int](/Api/DataType/Int.md) priority ，[LuaFunction]() func )</div>|
|:---------------------------------------------------------------------------------------|
|绑定`RenderStep`事件的`Lua`函数。[RenderPriority](/Api/Enumerate/UI/RenderPriority.md)为当前游戏内渲染层级，可根据需要进行插入|     

|<div style="width:925px">[void](/Api/DataType/Nil.md)&emsp; [<font color="dd00dd">UnbindFromRenderStep</font>](/Api/Class/Script/RunService_F/UnbindFromRenderStep.md)(&nbsp;[string](/Api/DataType/String.md) name  )</div>|
|:---------------------------------------------------------------------------------------|
|解除绑定`RenderStep`事件的`Lua`函数|     

|<div style="width:925px">[double](/Api/DataType/Double.md)&emsp; [<font color="dd00dd">CurrentMilliSecondTimeStamp</font>](/Api/Class/Script/RunService_F/CurrentMilliSecondTimeStamp.md)(&nbsp;  )</div>|
|:---------------------------------------------------------------------------------------|
|获取当前时间戳，精确到毫秒|     



------------------------------------------------------------------------------------------
## 事件（待确定)：

|<div style="width:925px">[SBXSignal](/Api/Parameter/SBXSignal.md)&emsp;[<font color="dd00dd">HeartBeat</font>](/Api/Class/Script/RunService_F/HeartBeat.md)( &nbsp;[double](/Api/DataType/Double.md) Step )</div></div>|
|:---------------------------------------------------------------------------------------|
|在物理模拟完成后每帧触发。      |

|<div style="width:925px">[SBXSignal](/Api/Parameter/SBXSignal.md)&emsp;[<font color="dd00dd">PostSimulation</font>](/Api/Class/Script/RunService_F/PostSimulation.md)( &nbsp;[double](/Api/DataType/Double.md) deltaTime )</div></div>|
|:---------------------------------------------------------------------------------------|
|在帧被模拟之后触发      |

|<div style="width:925px">[SBXSignal](/Api/Parameter/SBXSignal.md)&emsp;[<font color="dd00dd">PreRender</font>](/Api/Class/Script/RunService_F/PreRender.md)( &nbsp; [double](/Api/DataType/Double.md))</div></div>|
|:---------------------------------------------------------------------------------------|
|在帧被渲染之前触发      |


|<div style="width:925px">[SBXSignal](/Api/Parameter/SBXSignal.md)&emsp;[<font color="dd00dd">PreSimulation</font>](/Api/Class/Script/RunService_F/PreSimulation.md)( &nbsp; [double](/Api/DataType/Double.md))</div></div>|
|:---------------------------------------------------------------------------------------|
|在帧被模拟之前触发      |

|<div style="width:925px">[SBXSignal](/Api/Parameter/SBXSignal.md)&emsp;[<font color="dd00dd">RenderStepped</font>](/Api/Class/Script/RunService_F/RenderStepped.md)( &nbsp; [double](/Api/DataType/Double.md))</div></div>|
|:---------------------------------------------------------------------------------------|
|在帧被渲染之前每帧触发      |

|<div style="width:925px">[SBXSignal](/Api/Parameter/SBXSignal.md)&emsp;[<font color="dd00dd">Stepped</font>](/Api/Class/Script/RunService_F/Stepped.md)(&nbsp; [double](/Api/DataType/Double.md))</div></div>|
|:---------------------------------------------------------------------------------------|
|每次`Tick`触发`Stepped`事件      |



------------------------------------------------------------------------------------------
## 示例代码（需要完善)：

```lua
local RunService = game:GetService("RunService")
local ret = RunService:isClient()
```