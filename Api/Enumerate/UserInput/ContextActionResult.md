# ContextActionResult

枚举所属类：[ContextActionService](/Api/Class/Input/ContextActionService.md)

------------------------------------------------------------------------------------------
## 描述

控制着多个绑定动作的行为，可以用它给出的选项来设置某绑定动作对输入事件进行阻止还是放行，意思就是其他东西（包括其他绑定动作）可以对其进行处理

------------------------------------------------------------------------------------------
## 枚举

|<div style="width:200px">ContextActionResult</div>|<div style="width:100px"></div>|<div style="width:100px"></div>|
|:---   |:---|:---|
|**名称**   |**值**  |**描述**|
|Sink   |0   |如果`ContextActionService:BindAction`的`functionToBind`返回了`Enum.ContextActionResult.Sink`，那么输入事件就会停止于该函数，而其他位于其下的绑定动作则不会停止。这是默认的行为，前提是 functionToBind 没有返回任何值或者没有产生任何结果|
|Pass|1   |如果ContextActionService:BindAction的 functionToBind 返回了 Enum.ContextActionResult.Pass，那么就认为输入事件没有被 functionToBind 处理过，就会继续将输入事件传送到与相同的输入类型绑定的动作上。|

