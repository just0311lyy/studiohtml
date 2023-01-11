# BindContext
-----------------------------------------------------------------------------------------
## 描述

函数所属类：[ContextActionService](/Api/Class/Input/ContextActionService.md)

绑定一个回调函数到指定输入上

-----------------------------------------------------------------------------------------
## 参数

|<div style="width:200px">**名称**</div>|<div style="width:200px">**类型**</div>|<div style="width:200px">**默认**</div>|<div style="width:345px">**描述**</div>|
|:--------------------|:--------------------|:--------------------|:--------------------|
|actionName|[string](/Api/DataType/string.md)||自定义的名称，代表本次绑定|
|func|[LuaFunction](/Api/DataType/LuaFunction.md)||lua回调函数（三个参数1. `actionName`类型：[`string`](/Api/DataType/String.md)描述：最初传递给`BindAction` 的相同字符串;2.`state`类型：[`int`](/Api/DataType/Int.md)描述：当前事件的输入状态，等于[`UserInputState`](/Api/Enumerate/UserInput/UserInputState.md)中的值;3.`inputObj 类型：[`InputObject`](/Api/Class/Input/InputObject.md)描述：携带输入信息的对象）|
|createTouchBtn|[bool](/Api/DataType/Bool.md)||是否创建触摸按钮|
|hotkey|[ReflexVariant]()||快捷键|

## 返回

无返回值
