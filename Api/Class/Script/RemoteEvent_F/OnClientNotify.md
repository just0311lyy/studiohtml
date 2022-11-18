# ScriptObject （等待对齐）
-----------------------------------------------------------------------------------------
## 描述：

函数所属类：[RemotoEvent](/Api/Class/Script/RemoteEvent.md)

[RemoteEvent:FireServer](/Api/Class/Script/RemoteEvent_F/fireServer.md) 从一个 [LocalScript](/Api/Class/Script/LocalScriptNode.md) 中调用时触发 [Script](/Api/Class/Script/ScriptObject.md) 中的监听函数。

此事件用于取回由客户端向服务器触发的远程事件。此事件的目的是提供一种服务器与客户端通信的方法。

要从服务器向客户端触发，您应使用 [RemoteEvent:FireClient]() 和 [RemoteEvent.OnClientEvent]()。

-----------------------------------------------------------------------------------------
#### 示例代码：

```lua
	--只有是本地主机或者远程服务器才会执行下面的打印
	print("Hello, world")
```