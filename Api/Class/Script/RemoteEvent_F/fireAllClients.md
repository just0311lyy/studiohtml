# fireAllClient
-----------------------------------------------------------------------------------------
## 描述

函数所属类：[RemotoEvent](/Api/Class/Script/RemoteEvent.md)

`FireAllClients`函数在每个客户端触发 [RemoteEvent.OnClientEvent](/Api/Class/Script/RemoteEvent_F/OnClientNotify.md) 事件。

与 [RemoteEvent:FireClient](/Api/Class/Script/RemoteEvent_F/fireClient.md) 不同，此事件不接受目标玩家作为参数，而是在所有有连接至`OnClientEvent`事件的远程事件的客户端上触发。

因为此函数用于服务器向客户端通信，因此只能在 [Script](/Api/Class/Script/ScriptObject.md) 内起效。


- <font color="ff3333">注意：</font>
数据可以通过远程事件从服务器传递到客户端，就像数据从客户端传递到服务器一样。任何额外信息可作为`RemoteEvent:FireClient`和`FireAllClients`函数的参数传递。注意`FireClient`函数仍需要将发送信息的目标玩家作为第一项参数来传递。

-----------------------------------------------------------------------------------------
## 参数


|<div style="width:200px">名称</div>|<div style="width:200px">类型</div>|<div style="width:200px">默认</div>|<div style="width:200px">描述</div>|
|:--------------------|:--------------------|:--------------------|:--------------------|
|[argument]()      | [ReflexTuple](/Api/DataType/tuple.md) ||传入 [RemoteEvent.OnServerNotify](/Api/Class/Script/RemoteEvent_F/OnServerNotify.md) 方法的参数|


## 返回

无返回值

## 代码示例

```lua
print("1")

```