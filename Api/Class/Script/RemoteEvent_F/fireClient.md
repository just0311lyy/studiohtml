# FireClient 
-----------------------------------------------------------------------------------------
## 描述：

函数所属类：[RemotoEvent](/Api/Class/Script/RemoteEvent.md)

为指定的玩家触发 [RemoteEvent.OnClientEvent](/Api/Class/Script/RemoteEvent_F/OnClientNotify.md)。只有 [`LocalScript`](/Api/Class/Script/LocalScriptNode.md) 中在指定玩家的客户端上运行的连接会触发。与 [`RemoteFunction`](/Api/Class/Script/RemoteFunction.md) 类的区别在于后者会队列请求。

因为此函数用于服务器向客户端通信，因此只能在 Script 内起效。

* 注意

    * 数据可以通过远程事件从服务器传递到客户端，就像数据从客户端传递到服务器一样。任何额外信息可作为 [RemoteEvent:fireClient](/Api/Class/Script/RemoteEvent_F/fireClient.md) 和 fireAllClients 函数的参数传递。注意 FireClient 函数仍需要将发送信息的目标玩家作为第一项参数来传递。

    * 有时游戏需要从一个客户端向另一个客户端发送信息。MiniStudio 不支持客户端之间的直接联系，所以任何通信必须先经由服务器。这通常由远程事件完成（不过需要时也可以用函数）。首先，发送的客户端将调用 fireServer。在服务器端，连接至 OnServerNotify 的函数将监听到此触发，然后自身调用 fireClient。

-----------------------------------------------------------------------------------------
## 参数


|<div style="width:200px">名称</div>|<div style="width:200px">类型</div>|<div style="width:200px">默认</div>|<div style="width:200px">描述</div>|
|:--------------------|:--------------------|:--------------------|:--------------------|
|uin      | [int](/Api/DataType/Int.md) ||被事件所影响的[Player待定]()的uin|
|argument]     | [ReflexTuple](/Api/DataType/tuple.md) ||传入 [RemoteEvent.OnServerNotify](/Api/Class/Script/RemoteEvent_F/OnServerNotify.md) 方法的参数|


## 返回

无返回值

## 代码示例

```lua
print("1")

```