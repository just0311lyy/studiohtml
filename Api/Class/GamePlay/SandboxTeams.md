# Teams
------------------------------------------------------------------------------------------
## 描述

此类是一个服务！它是顶级单例，可以使用`GetService`函数获取。
[`Teams`](/Api/Class/GamePlay/SandboxTeams.md)服务用来存储游戏的[`Team`](/Api/Class/GamePlay/SandboxTeam.md)对象，这些[`Team`](/Api/Class/GamePlay/SandboxTeam.md)对象必须被设置为[`Teams`](/Api/Class/GamePlay/SandboxTeams.md)服务的子项。

继承：`ServiceNode` 

------------------------------------------------------------------------------------------
## 属性

------------------------------------------------------------------------------------------
## 函数

|<div style="width:1000px">[vector\<SandboxNode\>]() &emsp;[<font color="dd00dd">GetTeams</font> ](/Api/Class/GamePlay/SandboxTeams_F/GetTeams.md) ()</div>|
|:---|
|返回内含游戏[`Team`](/Api/Class/GamePlay/SandboxTeam.md)对象的表格。返回的[`Team`](/Api/Class/GamePlay/SandboxTeam.md)对象仅限[`Teams`](/Api/Class/GamePlay/SandboxTeams.md)服务的子对象。|


------------------------------------------------------------------------------------------
## 示例代码

```lua
local Teams = game:GetService('Teams')
local teamVector = Teams:GetTeams()
```