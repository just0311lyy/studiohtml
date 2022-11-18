# SandboxPostEffectService
------------------------------------------------------------------------------------------
## 描述

此类是一个服务！它是顶级单例，可以使用`GetService`函数获取。
`PostEffect`是一个用于后期处理效果的类。
继承：`ServiceNode` 

------------------------------------------------------------------------------------------
## 属性

------------------------------------------------------------------------------------------
## 函数

|<div style="width:500px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">addPostEffect</font>](/Api/Class/Effect/SandboxPostEffectService_F/addPostEffect.md) ([string](/Api/DataType/String.md) szName, [string](/Api/DataType/String.md) szMaterial, [string](/Api/DataType/String.md) szShader)</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|添加效果||||
|**参数名称**|**类别**|**默认**|**描述**|
|szName|string||效果标识符|
|szMaterial|string||效果素材|
|szShader|string||效果着色器|

|<div style="width:500px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">removePostEffect</font>](/Api/Class/Effect/SandboxPostEffectService_F/removePostEffect.md) ([string](/Api/DataType/String.md) szKey)</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|添加效果||||
|**参数名称**|**类别**|**默认**|**描述**|
|szKey|string||效果标识符|

|<div style="width:500px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">setParamValue</font>](/Api/Class/Effect/SandboxPostEffectService_F/setParamValue.md) ([string](/Api/DataType/String.md) szEffectName, [string](/Api/DataType/String.md) szName, [float](/Api/DataType/Float.md) fValue)</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|设置`PostEffect`参数||||
|**参数名称**|**类别**|**默认**|**描述**|
|szEffectName|string||效果名称|
|szName|string||效果标识符|
|fValue|float||效果值|

------------------------------------------------------------------------------------------
## 示例代码

```lua
local PostEffectService= game:GetService("PostEffectService")
```