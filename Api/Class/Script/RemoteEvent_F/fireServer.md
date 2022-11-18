# FireServer 
-----------------------------------------------------------------------------------------
## 描述：

函数所属类：[RemotoEvent](/Api/Class/Script/RemoteEvent.md)

FireServer 事件在服务器端用同样的参数触发 [RemoteEvent.OnServerNotify](/Api/Class/Script/RemoteEvent_F/OnServerNotify.md) 事件，前面外加一个玩家参数。

因为此函数用于客户端向服务器通信，因此只能在 [LocalScript](/Api/Class/Script/LocalScriptNode.md) 内起效。

请注意，当从客户端触发时，默认无需传递任何参数（不像从服务器向客户端触发时会传递玩家参数）。

-----------------------------------------------------------------------------------------
## 参数


|<div style="width:200px">名称</div>|<div style="width:200px">类型</div>|<div style="width:200px">默认</div>|<div style="width:200px">描述</div>|
|:--------------------|:--------------------|:--------------------|:--------------------|
|[argument]()      | [ReflexTuple](/Api/DataType/tuple.md)||传入 [RemoteEvent.OnServerNotify](/Api/Class/Script/RemoteEvent_F/OnServerNotify.md) 方法的参数|


## 返回

无返回值

## 代码示例

```lua
print("1")

```