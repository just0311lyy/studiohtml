# AnimatorLayer
------------------------------------------------------------------------------------------
## 描述

Animator Layer动画播放数据

*继承自*：
* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md)

------------------------------------------------------------------------------------------
## 属性

|<div style="width:1000px">[AnimationAsset](/Api/Class/Animation/SandboxAnimationAsset.md) &emsp;<font color="dd00dd">mask</font></div>|
|:---|
|当前的设备是否有可用的触摸屏|

------------------------------------------------------------------------------------------
## 函数

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp; <font color="dd00dd">Clear</font> ()</div>|
|:---|
|清空持有的Asset和清空加载|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsValid</font>](/Api/Class/Animation/SandboxAnimatorLayer_F/IsValid.md) ()</div>|
|:---|
|检测是否已经失效了（底层数据已经失效了）|


|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">CreateMotion</font>](/Api/Class/Animation/SandboxAnimatorLayer_F/CreateMotion.md) ([string](/Api/DataType/String.md) name, [AnimationAsset](/Api/Class/Animation/SandboxAnimationAsset.md) asset, [bool](/Api/DataType/Bool.md) isLoop)</div>|
|:---|
|创建一个动画切片|

|<div style="width:1000px"> vector<[AnimationAsset](/Api/Class/Animation/SandboxAnimationAsset.md)> &emsp;[<font color="dd00dd">GetMotions</font>](/Api/Class/Animation/SandboxAnimatorLayer_F/GetMotions.md) ()</div>|
|:---|
|获取当前持有的动画切片|

------------------------------------------------------------------------------------------
## 事件


------------------------------------------------------------------------------------------
## 示例代码

```lua
```