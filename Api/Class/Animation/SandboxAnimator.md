# Animator
------------------------------------------------------------------------------------------
## 描述

Animator 类

*继承自*：
* [AnimatorBase](/Api/Class/Animation/SandboxAnimatorBase.md)

------------------------------------------------------------------------------------------
## 属性

|<div style="width:1000px">[AnimatorController](/Api/Class/Animation/SandboxAnimatorController.md) &emsp;<font color="dd00dd">controller</font></div>|
|:---|
|对应的`controller`数据|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">pause</font></div>|
|:---|
|设置和获取是否暂停 (lua: pause field)|

------------------------------------------------------------------------------------------
## 函数

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp; <font color="dd00dd">Clear</font> ()</div>|
|:---|
|清空持有的Asset和清空加载|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsValid</font>](/Api/Class/Animation/SandboxAnimator_F/IsValid.md) ()</div>|
|:---|
|检测是否已经失效了（底层数据已经失效了）|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetControllerAsset</font>](/Api/Class/Animation/SandboxAnimator_F/SetControllerAsset.md) ([AnimationAsset](/Api/Class/Animation/SandboxAnimationAsset.md) asset)</div>|
|:---|
|设置对应的`controller`数据|

|<div style="width:1000px">[AnimatorController](/Api/Class/Animation/SandboxAnimatorController.md) &emsp;[<font color="dd00dd">NewController</font>](/Api/Class/Animation/SandboxAnimator_F/NewController.md) ([int](/Api/DataType/Int.md) type)</div>|
|:---|
|新建一个默认的状态机数据|

|<div style="width:1000px">[AnimationAsset](/Api/Class/Animation/SandboxAnimationAsset.md) &emsp;[<font color="dd00dd">GetSkeleton</font>](/Api/Class/Animation/SandboxAnimator_F/GetSkeleton.md) ()</div>|
|:---|
|获取当前的骨骼资源|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">Play</font>](/Api/Class/Animation/SandboxAnimator_F/Play.md) ([string](/Api/DataType/String.md) name, [int](/Api/DataType/Int.md) layer, [float](/Api/DataType/Float.md) normalized)</div>|
|:---|
|播放一个`state`|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">CrossFade</font>](/Api/Class/Animation/SandboxAnimator_F/CrossFade.md) ([string](/Api/DataType/String.md) name, [int](/Api/DataType/Int.md) layer, [float](/Api/DataType/Float.md) normalized)</div>|
|:---|
|`fade in`一个`state`|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetFloat</font>](/Api/Class/Animation/SandboxAnimator_F/CrossFade.md) ([string](/Api/DataType/String.md) key, [float](/Api/DataType/Float.md) value)</div>|
|:---|
|设置`animator params KV`值|

|<div style="width:1000px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">GetLayerCount</font>](/Api/Class/Animation/SandboxAnimator_F/GetLayerCount.md) ()</div>|
|:---|
|获取当前`layer`的个数|

|<div style="width:1000px">[AnimatorLayer](/Api/Class/Animation/SandboxAnimatorLayer.md) &emsp;[<font color="dd00dd">GetLayerByIndex</font>](/Api/Class/Animation/SandboxAnimator_F/GetLayerByIndex.md) ([int](/Api/DataType/Int.md) index)</div>|
|:---|
|按照`index`获取层级节点|

------------------------------------------------------------------------------------------
## 事件


------------------------------------------------------------------------------------------
## 示例代码

```lua
```