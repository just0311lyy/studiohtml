

# OverlapBox
-----------------------------------------------------------------------------------------
## 描述

函数所属类：[SandboxWorldService](/Api/Class/GamePlay/SandboxWorldService.md)

重叠框

-----------------------------------------------------------------------------------------
## 参数

|<div style="width:200px">**名称**</div>|<div style="width:200px">**类型**</div>|<div style="width:200px">**默认**</div>|<div style="width:345px">**描述**</div>|
|:--------------------|:--------------------|:--------------------|:--------------------|
|shape|[Vector3](/Api/DataType/Vector3.md)||长、宽、高的一半大小|
|pos|[Vector3](/Api/DataType/Vector3.md)||中心点的世界坐标|
|angle|[Vector3](/Api/DataType/Vector3.md)||朝向角度|
|isIgnoreTrigger|[bool](/Api/DataType/bool.md)||是否忽略trigger类型|
|filterGroup|[vector](/Api/DataType/vector.md)\<[int](/Api/DataType/int.md)\>||过滤组，{1，2，3} 含有的数字组会被查询|


## 返回

|<div style="width:200px">**返回类型**</div>|<div style="width:800px">**概要**</div>|
|:---|:---|
|[vector](/Api/DataType/vector.md)\<[ReflexMap](/Api/DataType/ReflexMap.md)\>|{isHit  ,normal ,position , distance ,obj}数组|