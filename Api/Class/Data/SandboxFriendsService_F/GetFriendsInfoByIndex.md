# GetFriendsInfoByIndex
-----------------------------------------------------------------------------------------
## 描述

函数所属类：[SandboxFriendsService](/Api/Class/Data/SandboxFriendsService.md)

根据好友的序列号拿到好友信息

-----------------------------------------------------------------------------------------
## 参数

|<div style="width:200px">**名称**</div>|<div style="width:200px">**类型**</div>|<div style="width:200px">**默认**</div>|<div style="width:345px">**描述**</div>|
|:--------------------|:--------------------|:--------------------|:--------------------|
|index|[int](/Api/DataType/Int.md)||好友数的序列号|

## 返回

|<div style="width:200px">**返回类型**</div>|<div style="width:800px">**概要**</div>|
|:---|:---|
|[ReflexTuple](/Api/Parameter/Tuple.md)|||好友信息 [`uin`(好友的`uin`), `nickName`(好友昵称), `onLine`(好友是否在线)]|