# OnServerInvoke
-----------------------------------------------------------------------------------------
## 描述

函数所属类：[RemoteFunction](/Api/Class/Script/RemoteFunction)

返回类型： [ReflexTuple](/Api/DataType/tuple.md)

当本地脚本[LocalScript]()使用[RemoteFunction.InvokeServer]()调用时，OnServerInvoke将会触发[Script]()中绑定的函数。当绑定的函数具有返回值时，对应的值也会返回至客户端。

此回调能够获取服务器触发的远程函数。其作用是为客户端与服务器之间提供通信方法。

- <font color="ff3333">注意：</font>

- 该函数绑定时需要使用 = 进行赋值，而不能使用事件的方法。

- 每次只能将一个函数赋值给OnServerInvoke，若分配多个函数，则会使用最新一次分配的函数


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