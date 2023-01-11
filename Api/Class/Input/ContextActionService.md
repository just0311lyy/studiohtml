# ContextActionService
------------------------------------------------------------------------------------------
## 描述

是一个服务，用于将用户输入动态绑定到上下文中，支持优先级绑定，优先级高的回调函数先调用

*继承自*：
* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md)

另请参阅：[UserInputService](/Api/Class/Animation/UserInputService.md)

------------------------------------------------------------------------------------------
## 属性


------------------------------------------------------------------------------------------
## 函数

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">BindActivate</font> ](/Api/Class/Input/ContextActionService_F/BindActivate.md) ([int](/Api/DataType/Int.md) userInputTypeForActivate, [int](/Api/DataType/Int.md) keyCodeForActivate)</div>|
|:---|
|绑定激活|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">UnbindActivate</font> ](/Api/Class/Input/ContextActionService_F/UnbindActivate.md) ([int](/Api/DataType/Int.md) userInputTypeForActivate, [int](/Api/DataType/Int.md) keyCodeForActivate)</div>|
|:---|
|绑定激活|

<<<<<<< HEAD
|<div style="width:500px">ReflexMap &emsp;[<font color="dd00dd">GetAllBoundActionInfo</font> ]() ()</div>|<div style="width:698px"></div>|
|:---|:---|
|（c++方法还未实现）||
|**返回类型**|**概要**|
|ReflexMap||

|<div style="width:500px">ReflexMap &emsp;[<font color="dd00dd">GetBoundActionInfo</font> ]() ([string](/Api/DataType/String.md) actionName)</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|（c++方法还未实现）||||
|**参数名称**|**类别**|**默认**|**描述**|
|actionName|string||自定义的名称，对应 BindAction 中使用的绑定名称|
|**返回类型**|||**概要**|
|ReflexMap||||
=======
|<div style="width:1000px">[ReflexMap](/Api/Parameter/ReflexMap.md) &emsp;[<font color="dd00dd">GetAllBoundActionInfo</font> ](/Api/Class/Input/ContextActionService_F/GetAllBoundActionInfo.md) ()</div>|
|:---|
|获取当前所有绑定的事件信息|

|<div style="width:1000px">[ReflexMap](/Api/Parameter/ReflexMap.md) &emsp;[<font color="dd00dd">GetBoundActionInfo</font> ](/Api/Class/Input/ContextActionService_F/GetBoundActionInfo.md) ([string](/Api/DataType/String.md) actionName)</div>|
|:---|
|获取当前绑定`actionName`的事件信息|

|<div style="width:1000px">[SandboxNode](/Api/Class/NoType/SandboxNode.md) &emsp;[<font color="dd00dd">GetButton</font> ](/Api/Class/Input/ContextActionService_F/GetButton.md) ([string](/Api/DataType/String.md) actionName)</div>|
|:---|
|通过绑定名称获取该按钮节点|

|<div style="width:1000px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">GetCurrentLocalToolIcon</font> ](/Api/Class/Input/ContextActionService_F/GetCurrentLocalToolIcon.md) ()</div>|
|:---|
|获取当前本地`tool`图片|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetDescription</font>](/Api/Class/Input/ContextActionService_F/SetDescription.md) ([string](/Api/DataType/String.md) actionName, [string](/Api/DataType/String.md) description)</div>|
|:---|
|设置描述|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetImage</font>](/Api/Class/Input/ContextActionService_F/SetImage.md) ([string](/Api/DataType/String.md) actionName, [string](/Api/DataType/String.md) image)</div>|
|:---|
|设置图片|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetPosition</font>](/Api/Class/Input/ContextActionService_F/SetPosition.md) ([string](/Api/DataType/String.md) actionName, [Vector2](/Api/DataType/Vector2.md) position)</div>|
|:---|
|设置位置|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetTitle</font>](/Api/Class/Input/ContextActionService_F/SetTitle.md) ([string](/Api/DataType/String.md) actionName, [string](/Api/DataType/String.md) title)</div>|
|:---|
|设置标题|
>>>>>>> origin/main


|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">BindContext</font> ](/Api/Class/Input/ContextActionService_F/BindContext.md) ([string](/Api/DataType/String.md) actionName, [LuaFunction]() func, [bool](/Api/DataType/Bool.md) createTouchBtn, [ReflexVariant]() hotkey)</div>|
|:---|
|绑定一个回调函数到指定输入上|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">BindContextAtPriority</font> ](/Api/Class/Input/ContextActionService_F/BindContextAtPriority.md) ([string](/Api/DataType/String.md) actionName, [LuaFunction]() func, [bool](/Api/DataType/Bool.md) createTouchBtn, [int](/Api/DataType/Int.md) priority, [ReflexVariant]() hotkey)</div>|
|:---|
|绑定一个回调函数到指定输入上，并指定优先级|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">UnbindContext</font> ](/Api/Class/Input/ContextActionService_F/UnbindContext.md) ([string](/Api/DataType/String.md) actionName)</div>|
|:---|
|取消指定的用户绑定|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">UnbindAllContext</font>]()</div>|
|:---|
|移除所有的函数绑定|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">BindAction</font> ](/Api/Class/Input/ContextActionService_F/BindAction.md) ([string](/Api/DataType/String.md) actionName, [LuaFunction]() func, [int](/Api/DataType/Int.md) nActionType, [int](/Api/DataType/Int.md) nSubType)</div>|
|:---|
|绑定一个回调函数到指定输入上，`(准备废弃接口，不推荐使用了，推荐使用 BindContext 这套新接口)`|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">BindActionAtPriority</font> ](/Api/Class/Input/ContextActionService_F/BindActionAtPriority.md) ([string](/Api/DataType/String.md) actionName, [LuaFunction]() func, [int](/Api/DataType/Int.md) priority, [int](/Api/DataType/Int.md) nActionType, [int](/Api/DataType/Int.md) nSubType)</div>|
|:---|
|绑定一个回调函数到指定输入上，并指定优先级`(准备废弃接口，不推荐使用了，推荐使用 BindContext 这套新接口)`|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">UnbindAction</font> ](/Api/Class/Input/ContextActionService_F/UnbindAction.md) ([string](/Api/DataType/String.md) actionName)</div>|
|:---|
|取消指定的用户绑定`(准备废弃接口，不推荐使用了，推荐使用 BindContext 这套新接口)`|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">UnbindAllActions</font>]()</div>|
|:---|
|移除所有的函数绑定`(准备废弃接口，不推荐使用了，推荐使用 BindContext 这套新接口)`|


------------------------------------------------------------------------------------------
## 事件


------------------------------------------------------------------------------------------
## 示例代码

```lua
local ContextActionService = game:GetService("ContextActionService")
local curActionName = "moveForwardAction"
local function handleMoveForward(actionName, inputState, inputObj)
    print(actionName)     -- 打印 moveForwardAction
    if inputState == Enum.UserInputState.InputBegin.Value then
        self.ForwardBackValue = 1
    else
        self.ForwardBackValue = 0
    end
    self.LocalCharacter:Move(Vector3.New(self.LeftRightValue,0,self.ForwardBackValue),true)
end
ContextActionService:BindAction(
    curActionName, 
    handleMoveForward, 
    Enum.ContextActionType.KeyBoard.Value, 
    Enum.KeyCode.W.Value )
```