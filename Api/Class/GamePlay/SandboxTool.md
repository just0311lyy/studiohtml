# Tool
------------------------------------------------------------------------------------------
## 描述：

在桌面端，按数字键 (1 - 8) 会切换装备已有的工具

*继承自*：
* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md)

------------------------------------------------------------------------------------------
## 属性：

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CanBeDropped</font></div>|
|:---|
|可否丢弃Tool，默认不可以丢弃|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Enabled</font></div>|
|:---|
|决定Tool能否被使用，默认可以使用|

|<div style="width:1000px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">GripPos</font></div>|
|:---|
|夹点位置|

|<div style="width:1000px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">GripEuler</font></div>|
|:---|
|夹点的欧拉|

|<div style="width:1000px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">ToolTip</font></div>|
|:---|
|tool提示信息|

|<div style="width:1000px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">TextureId</font></div>|
|:---|
|默认快捷栏界面，显示的图标资源|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;<font color="dd00dd">Index</font></div>|
|:---|
|快捷栏下标|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">EquippedValue</font></div>|
|:---|
|是否装备（不允许访问）|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">ActivatedValue</font></div>|
|:---|
|是否激活（不允许访问）|

------------------------------------------------------------------------------------------
## 函数

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Activate</font>  ( )</div>|
|:---|
|已装备的的工具，模拟点击使用，会触发`Activated`事件。返回true，表示成功触发|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">Deactivate</font>  ( )</div>|
|:---|
|模拟工具的结束使用.返回true，表示模拟工具结束使用成功|

------------------------------------------------------------------------------------------
## 事件

|<div style="width:1125px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;<font color="dd00dd">Activated</font>( )</div>|
|:---|
|玩家已装备工具，点击鼠标左键时触发|

|<div style="width:1125px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;<font color="dd00dd">Deactivated</font>( )</div>|
|:---|
|当鼠标左键松开时触发。|

|<div style="width:1125px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;<font color="dd00dd">Equipped</font>( )</div>|
|:---|
|当载入Tool时触发。|

|<div style="width:1125px">[SBXSignal](/Api/Parameter/SBXSignal.md) &emsp;<font color="dd00dd">Unequipped</font>( )</div>|
|:---|
|当卸载Tool时触发。|


------------------------------------------------------------------------------------------
## 示例代码

* **示例代码1：**

在`StarterPack`下新增一个[`Tool`](/Api/Class/GamePlay/SandboxTool.md)节点，[`Tool`](/Api/Class/GamePlay/SandboxTool.md)下新增一个[`Script`](/Api/Class/Script/ScriptObject.md)节点，运行游戏，按1装备该[`Tool`](/Api/Class/GamePlay/SandboxTool.md)，鼠标点击空白处使用。

```lua
local tool = script.Parent
tool.Equipped:connect(function()
        print("Equipped----")
    end
)
tool.Unequipped:connect(function()
        print("Unequipped----")
    end
)
tool.Activated:Connect(function()
        print("Activated----")
    end
)
tool.Deactivated:Connect(function()
        print("Deactivated----")
    end
)
tool.TouchBegin:connect(function()
        print("onTouchBegin----")
    end
)
tool.TouchEnd:connect(function()
        print("onTouchEnd----")
    end
)
```

* **示例代码2：**

以下示例是使用[`LocalPlayer`](/Api/Class/GamePlay/SandBoxLocalPlayer.md)的`EquipTool`，`UnequipTools`接口，装备指定[`Tool`](/Api/Class/GamePlay/SandboxTool.md)和卸下[`Tool`](/Api/Class/GamePlay/SandboxTool.md) 的示例。<br>
将其放到[`Tool`](/Api/Class/GamePlay/SandboxTool.md)下的[`Script`](/Api/Class/Script/ScriptObject.md)节点里，按X装备该[`Tool`](/Api/Class/GamePlay/SandboxTool.md)，按Z卸下当前的装备（不管是不是该[`Tool`](/Api/Class/GamePlay/SandboxTool.md)节点）

```lua
local tool = script.Parent
local playersService = game:GetService("Players")
local localPlayer = playersService.LocalPlayer

local ContextActionService = game:GetService("ContextActionService")

local function testEquipTool(actionName, inputState, inputObj)
    if inputState == Enum.UserInputState.InputBegin.Value then
        localPlayer:EquipTool( tool )
    end
end
ContextActionService:BindAction(
    "testEquipTool", 
    testEquipTool, 
    Enum.ContextActionType.KeyBoard.Value, 
    string.byte('X') )

local function testUnequipTool(actionName, inputState, inputObj)
    if inputState == Enum.UserInputState.InputBegin.Value then
        localPlayer:UnequipTools()
    end
end

ContextActionService:BindAction(
    "testUnequipTool", 
    testUnequipTool, 
    Enum.ContextActionType.KeyBoard.Value, 
    string.byte('Z') )
```