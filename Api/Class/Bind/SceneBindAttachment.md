# BindAttachment
------------------------------------------------------------------------------------------
## 描述

给节点添加绑点，一节点挂在绑点上，会相对于其父节点一起改变

*继承自*：
* [SceneTransObject](/Api/Class/NoType/SceneTransObject.md)

------------------------------------------------------------------------------------------
## 属性

|<div style="width:1000px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">BoneName</font></div>|
|:---|
|绑点名字|

|<div style="width:1000px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">Position</font></div>|
|:---|
|绑点坐标 (`Rainbow::Vector3f`)|

|<div style="width:1000px">[Vector3](/Api/DataType/Vector3.md) &emsp;<font color="dd00dd">Euler</font></div>|
|:---|
|绑点欧拉角 (`Rainbow::Vector3f`)|

|<div style="width:1000px">[string](/Api/DataType/String.md) &emsp;<font color="dd00dd">ModelId</font></div>|
|:---|
|绑点模型Id|

|<div style="width:1000px">[bool](/Api/DataType/Bool.md) &emsp;<font color="dd00dd">RelpaceBoneModel</font></div>|
|:---|
|绑点替代的骨骼模型|

------------------------------------------------------------------------------------------
## 函数


------------------------------------------------------------------------------------------
## 示例代码

```lua
--创建模型
local model = SandboxNode.new('SceneModelObject', game.WorkSpace)
model.ModelId = string.format("sandboxAsset://entity/%s/body.omod","100041")
model.Position = Vector3.new(500, 700, 150)
--给模型设置绑点
local attachment= SandboxNode.new('SceneBindAttachment', model)
attachment.BoneName = 'attachment'
attachment.LocalPosition = Vector3.new(100, 0, 100)
attachment.LocalScale = Vector3.new(2, 1, 1)
```