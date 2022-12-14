# PostEffectService
------------------------------------------------------------------------------------------
## 描述

此类是一个服务！它是顶级单例，可以使用`GetService`函数获取。
`PostEffect`是一个用于后期处理效果的类。

*继承自*：
* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md) 

------------------------------------------------------------------------------------------
## 属性

------------------------------------------------------------------------------------------
## 函数

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">addPostEffect</font>](/Api/Class/Effect/SandboxPostEffectService_F/addPostEffect.md) ([string](/Api/DataType/String.md) szName, [string](/Api/DataType/String.md) szMaterial, [string](/Api/DataType/String.md) szShader)</div>|
|:---|
|添加效果|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">removePostEffect</font>](/Api/Class/Effect/SandboxPostEffectService_F/removePostEffect.md) ([string](/Api/DataType/String.md) szKey)</div>|
|:---|
|移除|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">setParamValue</font>](/Api/Class/Effect/SandboxPostEffectService_F/setParamValue.md) ([string](/Api/DataType/String.md) szEffectName, [string](/Api/DataType/String.md) szName, [float](/Api/DataType/Float.md) fValue)</div>|
|:---|
|设置`PostEffect`参数|

------------------------------------------------------------------------------------------
## 示例代码

```lua
local PostEffectService= game:GetService("PostEffectService")
```