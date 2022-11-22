

# SweepCapsule
-----------------------------------------------------------------------------------------
## 描述

函数所属类：[SandboxWorldService](/Api/Class/GamePlay/SandboxWorldService.md)

扫描胶囊

-----------------------------------------------------------------------------------------
## 参数

|<div style="width:200px">**名称**</div>|<div style="width:200px">**类型**</div>|<div style="width:200px">**默认**</div>|<div style="width:345px">**描述**</div>|
|:--------------------|:--------------------|:--------------------|:--------------------|
|radius|[float](/Api/DataType/float.md)||半径|
|p0|[Vector3](/Api/DataType/Vector3.md)||胶囊体上面的球体的中心点|
|p1|[Vector3](/Api/DataType/Vector3.md)||胶囊体下面的球体的中心点|
|dir|[Vector3](/Api/DataType/Vector3.md)||朝向|
|distance|[float](/Api/DataType/float.md)||检测距离|
|isIgnoreTrigger|[bool](/Api/DataType/bool.md)||是否忽略trigger类型|
|filterGroup|[vector](/Api/DataType/vector.md)\<[int](/Api/DataType/int.md)\>||过滤组，{1，2，3} 含有的数字组会被查询|

## 返回

|<div style="width:200px">**返回类型**</div>|<div style="width:800px">**概要**</div>|
|:---|:---|
|[ReflexMap](/Api/DataType/ReflexMap.md)|{isHit  ,normal ,position , distance ,obj}|
