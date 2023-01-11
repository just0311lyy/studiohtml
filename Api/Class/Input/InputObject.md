# InputObject 
------------------------------------------------------------------------------------------
## 描述

在用户输入事件触发时，描述具体的输入信息的对象，例如鼠标位置，按键信息等

------------------------------------------------------------------------------------------
## 属性

|<div style="width:1000px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">Delta</font>]()</div>|
|:---|
|暂无信息|

|<div style="width:1000px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">Position</font>]()</div>|
|:---|
|鼠标相关的事件中，描述鼠标的位置|


|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">KeyCode</font>]()</div>|
|:---|
|按键事件触发时，对应的按键码，等于`Enum.KeyCode`中的某个值|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">UserInputState</font>]()</div>|
|:---|
|描述输入状态（开始，结束等）等于枚举[`UserInputState`](/Api/Enumerate/UserInput/UserInputState.md)中的某个值|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">UserInputType</font>]()</div>|
|:---|
|描述输入的类型 等于枚举[`UserInputType`](/Api/Enumerate/UserInput/UserInputType.md)中的某个值|

------------------------------------------------------------------------------------------
## 函数

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsModifierKeyDown</font> ](/Api/Class/Input/InputObject_F/IsModifierKeyDown.md) ([int](/Api/DataType/Int.md) vkey)</div>|
|:---|
|按键是否按下|


