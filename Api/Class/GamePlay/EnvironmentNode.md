# EnvironmentNode
------------------------------------------------------------------------------------------
## 描述

环境节点，可以设置天气，星球、重力和时间

*继承自*：
* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md)

------------------------------------------------------------------------------------------
## 属性：

|<div style="width:1000px">[EnumWeather](/Api/Enumerate/GamePlay/EnumWeather.md) &emsp;[<font color="dd00dd">Weather</font>]()</div>|
|:---|
|设置天气类型的枚举，有晴天、雨天、打雷和自定义。参见枚举[EnvironmentNode::EnumWeather](/Api/Enumerate/GamePlay/EnumWeather.md)|

|<div style="width:1000px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">Gravity</font>]()</div>|
|:---|
|环境重力设置|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">TimeHour</font>]()</div>|
|:---|
|时间设置|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">LockTimeHour</font>]()</div>|
|:---|
|是否锁定时间|

|<div style="width:1000px">[EnumSkyPlanet](/Api/Enumerate/GamePlay/EnumSkyPlanet.md) &emsp;[<font color="dd00dd">SkyPlanet</font>]()</div>|
|:---|
|设置星球类型的枚举，有地球、萌眼星、烈焰星、火山和自定义。参见枚举[EnvironmentNode::EnumSkyPlanet](/Api/Enumerate/GamePlay/EnumSkyPlanet.md)|

|<div style="width:1000px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">SkyPlanetRes</font>]()</div>|
|:---|
|设置天空|

------------------------------------------------------------------------------------------
## 函数：

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">LockTime</font> ](/Api/Class/GamePlay/EnvironmentNode_F/LockTime.md) ([int](/Api/DataType/Int.md) timehour)</div>|
|:---|
|锁定时间|

------------------------------------------------------------------------------------------
## 事件：

|<div style="width:500px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;[<font color="dd00dd">WeatherChanged</font> ]() ( [int](/Api/DataType/Int.md) Weather )</div>|<div style="width:698px"></div>|
|:---|:---|
|天气改变时触发||
|**返回类型**|**概要**|
|int|天气枚举`EnumWeather`对应的`int`值|


|<div style="width:500px">[SBXSignal>]() &emsp;[<font color="dd00dd">GravityChanged</font> ]() ( [float](/Api/DataType/Float.md) Garvity )</div>|<div style="width:698px"></div>|
|:---|:---|
|重力改变时触发||
|**返回类型**|**概要**|
|float|重力值|

|<div style="width:500px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;[<font color="dd00dd">SkyPlanetChanged</font> ]()( [int](/Api/DataType/Int.md) SkyBox )</div>|<div style="width:698px"></div>|
|:---|:---|
|天空盒改变时触发||
|**返回类型**|**概要**|
|int|天空包围盒枚举`EnumSkyPlanet`对应的`int`值|

|<div style="width:500px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;[<font color="dd00dd">TimeChanged</font> ]() ( [int](/Api/DataType/Int.md) Time )</div>|<div style="width:698px"></div>|
|:---|:---|
|时间改变时触发||
|**返回类型**|**概要**|
|int|24小时制中的某一小时值|

------------------------------------------------------------------------------------------
## 示例代码：

```lua
 local workspace = game:GetService("workspace")
 local environment = workspace.Environment
 --设置天气为下雨
 environment.Weather = Enum.EnumWeather.Rain
 --设置天空为火山
 environment.SkyPlanet = Enum.EnumSkyPlanet.Volcano
 --设置时间为22
 environment.TimeHour = 22
 ```
