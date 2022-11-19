# SandboxTeams
------------------------------------------------------------------------------------------
## 描述

此类是一个服务！它是顶级单例，可以使用`GetService`函数获取。
`Teams`服务用来存储游戏的`Team`对象，这些`Team`对象必须被设置为`Teams`服务的子项。

继承：`ServiceNode` 

------------------------------------------------------------------------------------------
## 属性

------------------------------------------------------------------------------------------
## 函数

|<div style="width:500px">[vector\<SandboxNode\>]() &emsp;[<font color="dd00dd">GetTeams</font> ](/Api/Class/GamePlay/SandboxTeams_F/GetTeams.md) ()</div>|<div style="width:698px"></div>|
|:---|:---|
|返回内含游戏`Team`对象的表格。返回的`Team`对象仅限`Teams`服务的子对象。||
|**返回类型**|**概要**|
|vector\<SandboxNode\>|返回内含游戏`Team`对象的表格|


------------------------------------------------------------------------------------------
## 示例代码

```lua
local Teams = game:GetService('Teams')
local teamVector = Teams:GetTeams()
```