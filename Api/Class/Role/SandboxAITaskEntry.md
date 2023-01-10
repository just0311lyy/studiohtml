# AITaskEntry
------------------------------------------------------------------------------------------
## 描述

`AITaskEntry`

*继承自*：
* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md)

------------------------------------------------------------------------------------------
## 属性

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CanInterrupted</font></div>|
|:---|
|是否可以中断|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">CanRun</font></div>|
|:---|
|是否可以继续|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;<font color="dd00dd">Priority</font></div>|
|:---|
|优先级|

------------------------------------------------------------------------------------------
## 函数

------------------------------------------------------------------------------------------
## 事件

|<div style="width:1000px">[SBXSignal]() &emsp;[<font color="dd00dd">Run</font> ]() ()</div>|
|:---|
|lua任务运行时触发|

|<div style="width:1000px">[SBXSignal]() &emsp;[<font color="dd00dd">Start</font> ]() ()</div>|
|:---|
|lua任务开始执行时触发|

|<div style="width:1000px">[SBXSignal]() &emsp;[<font color="dd00dd">Ready</font> ]() ()</div>|
|:---|
|lua任务完成时触发|

|<div style="width:1000px">[SBXSignal]() &emsp;[<font color="dd00dd">Tick</font> ]() ()</div>|
|:---|
|lua任务循环时触发|

|<div style="width:1000px">[SBXSignal]() &emsp;[<font color="dd00dd">Reset</font> ]() ()</div>|
|:---|
|lua任务重置时触发|

|<div style="width:1000px">[SBXSignal]() &emsp;[<font color="dd00dd">Destroy</font> ]() ()</div>|
|:---|
|lua任务销毁时触发|

------------------------------------------------------------------------------------------
## 示例代码

```lua


```