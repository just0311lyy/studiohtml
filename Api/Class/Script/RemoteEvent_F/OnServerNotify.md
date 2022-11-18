# OnServerNotify
-----------------------------------------------------------------------------------------
## 描述：

函数所属类：[RemotoEvent](/Api/Class/Script/RemoteEvent.md)


RemoteEvent:FireServer 从一个  [`LocalScript`](/Api/Class/Script/LocalScriptNode.md) 中调用时触发 [Script](/Api/Class/Script/ScriptObject.md)中的监听函数。

此事件用于取回由客户端向服务器触发的远程事件。此事件的目的是提供一种服务器与客户端通信的方法，在这篇文章中有详细描述。此事件取回由客户端向服务器触发的远程事件。

要从服务器向客户端触发，您应使用 [RemoteEvent:fireClient](/Api/Class/Script/RemoteEvent_F/fireClient.md) 和 [RemoteEvent.OnClientNotify](/Api/Class/Script/RemoteEvent_F/OnServerNotify.md)。

-----------------------------------------------------------------------------------------
## 参数


|<div style="width:200px">名称</div>|<div style="width:200px">类型</div>|<div style="width:200px">默认</div>|<div style="width:200px">描述</div>|
|:--------------------|:--------------------|:--------------------|:--------------------|
|uin      | [int](/Api/DataType/Int.md) ||与其相关联的的[Player待定]()的uin|
|argument      | [Turple](/Api/Parameter/Tuple.md) ||fireServer传递的参数|


## 返回

无返回值

## 代码示例

```lua
print("1")
