# Animation
------------------------------------------------------------------------------------------
## 描述

动画系统基类

*继承自*：
* [AnimatorBase](/Api/Class/Animation/SandboxAnimatorBase.md)

------------------------------------------------------------------------------------------
## 属性

------------------------------------------------------------------------------------------
## 函数

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsValid</font>](/Api/Class/Animation/SandboxAnimation_F/IsValid.md)</div>|
|:---|
|检测是否已经失效了（底层数据已经失效了）|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp; <font color="dd00dd">Clear</font> </div>|
|:---|
|清空持有的Asset和清空加载|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsPlaying</font>](/Api/Class/Animation/SandboxAnimation_F/IsPlaying.md) ([string](/Api/DataType/String.md) clipName)</div>|
|:---|
|是否正在播放某个切片|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">Stop</font>](/Api/Class/Animation/SandboxAnimation_F/Stop.md) ([string](/Api/DataType/String.md) clipName)</div>|
|:---|
|停止某个动画切片播放|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetSpeed</font>](/Api/Class/Animation/SandboxAnimation_F/SetSpeed.md) ([string](/Api/DataType/String.md) clipName, [float](/Api/DataType/Float.md) speed)</div>|
|:---|
|设置某个动画切片播放速度|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">Rewind</font>](/Api/Class/Animation/SandboxAnimation_F/Rewind.md) ([string](/Api/DataType/String.md) clipName)</div>|
|:---|
|设置某个动画从头开始播放|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetWrapMode</font>](/Api/Class/Animation/SandboxAnimation_F/SetWrapMode.md) ([string](/Api/DataType/String.md) clipName, [AnimationWrapMode](/Api/Enumerate/Animation/AnimationWrapMode.md) mode)</div>|
|:---|
|设置某个动画切片wrap模式（动画边缘处理）|

|<div style="width:1000px"> vector<[AnimationAsset](/Api/Class/Animation/SandboxAnimationAsset.md)> &emsp;[<font color="dd00dd">GetClips</font>](/Api/Class/Animation/SandboxAnimation_F/GetClips.md) ()</div>|
|:---|
|获取当前animation持有的所有动画切片资源|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetClips</font>](/Api/Class/Animation/SandboxAnimation_F/SetClips.md) (vector<[AnimationAsset](/Api/Class/Animation/SandboxAnimationAsset.md)>)</div>|
|:---|
|设置当前animation持有的动画切片资源|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetDefaultClip</font>](/Api/Class/Animation/SandboxAnimation_F/SetDefaultClip.md) ([AnimationAsset](/Api/Class/Animation/SandboxAnimationAsset.md) asset)</div>|
|:---|
|设置默认的动画切片（如果没有持有则会新增持有）|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">Play</font>](/Api/Class/Animation/SandboxAnimation_F/Play.md) ([string](/Api/DataType/String.md) clipName, [AnimationPlayMode](/Api/Enumerate/Animation/AnimationPlayMode.md) mode)</div>|
|:---|
|播放切片|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">Blend</font>](/Api/Class/Animation/SandboxAnimation_F/Blend.md) ([string](/Api/DataType/String.md) clipName, [float](/Api/DataType/Float.md) targetWeight, [float](/Api/DataType/Float.md) time)</div>|
|:---|
|设置切片动画混合权重|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">CrossFade</font>](/Api/Class/Animation/SandboxAnimation_F/CrossFade.md) ([string](/Api/DataType/String.md) clipName, [float](/Api/DataType/Float.md) targetWeight, [AnimationPlayMode](/Api/Enumerate/Animation/AnimationPlayMode.md) mode)</div>|
|:---|
|设置切片动画渐变（fade）|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">AddClip</font>](/Api/Class/Animation/SandboxAnimation_F/AddClip.md) ([AnimationAsset](/Api/Class/Animation/SandboxAnimationAsset.md) asset, [string](/Api/DataType/String.md) name, [int](/Api/DataType/Int.md) firstFrame, [int](/Api/DataType/Int.md) lastFrame, [bool](/Api/DataType/Bool.md) loop)</div>|
|:---|
|添加一个切片动画|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">RemoveClip</font>](/Api/Class/Animation/SandboxAnimation_F/RemoveClip.md) ([string](/Api/DataType/String.md) clipName)</div>|
|:---|
|移除一个切片动画|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">GetAutoPlay</font>](/Api/Class/Animation/SandboxAnimation_F/GetAutoPlay.md) ()</div>|
|:---|
|获取是否自动播放|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">SetAutoPlay</font>](/Api/Class/Animation/SandboxAnimation_F/SetAutoPlay.md) ([bool](/Api/DataType/Bool.md) autoPlay)</div>|
|:---|
|设置是否自动播放|

------------------------------------------------------------------------------------------
## 事件


------------------------------------------------------------------------------------------
## 示例代码

```lua
```