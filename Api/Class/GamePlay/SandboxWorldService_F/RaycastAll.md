
# RaycastAll
-----------------------------------------------------------------------------------------
## 描述

函数所属类：[SandboxWorldService](/Api/Class/GamePlay/SandboxWorldService.md)

射线段检测，返回所有碰撞物，最多128个

-----------------------------------------------------------------------------------------
## 参数

|<div style="width:200px">**名称**</div>|<div style="width:200px">**类型**</div>|<div style="width:200px">**默认**</div>|<div style="width:345px">**描述**</div>|
|:--------------------|:--------------------|:--------------------|:--------------------|
|origin|[Vector3](/Api/DataType/Vector3.md)||射线段的起点，世界坐标|
|unitDir|[Vector3](/Api/DataType/Vector3.md)||射线段的世界方向，单位向量|
|distance|[float](/Api/DataType/float.md)||射线段的最大长度|
|isIgnoreTrigger|[bool](/Api/DataType/bool.md)||是否忽略trigger类型|
|filterGroup|[vector](/Api/DataType/vector.md)\<[int](/Api/DataType/int.md)\>||过滤组，{1，2，3} 含有的数字组会被查询|


## 返回

|<div style="width:200px">**返回类型**</div>|<div style="width:800px">**概要**</div>|
|:---|:---|
|[vector](/Api/DataType/vector.md)\<[ReflexMap](/Api/DataType/ReflexMap.md)\>|所有碰撞物|
