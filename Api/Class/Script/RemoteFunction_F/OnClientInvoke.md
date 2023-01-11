# OnClientInvoke
-----------------------------------------------------------------------------------------
## 描述

函数所属类：[RemoteFunction](/Api/Class/Script/RemoteFunction)

返回类型： [ReflexTuple](/Api/DataType/tuple.md)

当服务器脚本[Script]()使用[RemoteFunction.InvokeClient]()调用时，OnClientInvoke将会触发[LocalScript]()中绑定的函数。当绑定的函数具有返回值时，对应的值也会返回值服务器。

此回调能够监听服务器向客户端所调用的远程函数。其作用是为客户端与服务器之间提供通信方法。



-----------------------------------------------------------------------------------------
## 参数


|<div style="width:200px">名称</div>|<div style="width:200px">类型</div>|<div style="width:200px">默认</div>|<div style="width:200px">描述</div>|
|:--------------------|:--------------------|:--------------------|:--------------------|
|arguments    | [ReflexTuple](/Api/DataType/tuple.md) ||传入 [RemoteFunction.OnClientInvoke]() 方法的参数|


## 返回

|<div style="width:400px">类型</div>|<div style="width:400px">描述</div>|
|:--------------------|:--------------------|
|[ReflexTuple](/Api/DataType/tuple.md)   |[RemoteFunction.OnClientInvoke]()函数的返回值|

## 代码示例

```lua
print("1")

```