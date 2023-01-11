# AnimationAsset
------------------------------------------------------------------------------------------
## 描述

动画资源节点

*继承自*：
* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md)

------------------------------------------------------------------------------------------
## 属性

------------------------------------------------------------------------------------------
## 函数

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">Ready</font>](/Api/Class/Animation/SandboxAnimationAsset_F/Ready.md)</div>|
|:---|
|资源是否已经加载完成或者已经持有了资源|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">Load</font>](/Api/Class/Animation/SandboxAnimationAsset_F/Load.md) ([AnimationType](/Api/Enumerate/Animation/AnimationType.md) loadType, [string](/Api/DataType/String.md) assetId)</div>|
|:---|
|加载动画|

|<div style="width:1000px">[void](/Api/Parameter/void.md) &emsp;[<font color="dd00dd">Clear</font>]()</div>|
|:---|
|清空持有的Asset和清空加载|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">IsLoadSuccess</font>](/Api/Class/Animation/SandboxAnimationAsset_F/IsLoadSuccess.md)</div>|
|:---|
|判断当前是否加载成功|

|<div style="width:1000px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">GetLoadAssetId</font>](/Api/Class/Animation/SandboxAnimationAsset_F/GetLoadAssetId.md)</div>|
|:---|
|获取当前加载中或者已加载的`assetId`|

|<div style="width:1000px">[AnimationType](/Api/Enumerate/Animation/AnimationType.md) &emsp;[<font color="dd00dd">GetResType</font>](/Api/Class/Animation/SandboxAnimationAsset_F/GetResType.md)</div>|
|:---|
|获取当前持有的资源类型或者正在加载的资源类型|


------------------------------------------------------------------------------------------
## 事件

|<div style="width:500px">[SBXSignal\<[bool](/Api/DataType/Bool.md)\>]() &emsp;[<font color="dd00dd">GetLoadFinish</font> ]() ()</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|获取当前异步加载的通知||||
|**返回类型**|||**概要**|
|SBXSignal|||当前异步加载的通知，事件参数为（`bool isFinish`）|
|**SBXSignal参数名称**|**类别**|**默认**|**描述**|
|isFinish|bool||`true`为加载完成|

------------------------------------------------------------------------------------------
## 示例代码

```lua
```