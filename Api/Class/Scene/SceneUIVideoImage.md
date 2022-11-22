# SceneUIVideoImage
------------------------------------------------------------------------------------------
## 描述

图片格式可以是`MP4`类型的

*继承自*：
* [SceneUIComponent](/Api/Class/Scene/SceneUIComponent.md)

------------------------------------------------------------------------------------------
## 属性

|<div style="width:1125px">[string](/Api/DataType/String.md) &emsp;[<font color="dd00dd">Icon</font>](/Api/Class/Scene/SceneUIVideoImage_F/Icon.md)</div>|
|:---|
|图片的路径。|

------------------------------------------------------------------------------------------
## 示例代码

```lua
local workspace = game:GetService("workspace")
local root = SandboxNode.new('SceneUIRoot',workspace)
local npcOneVideo = SandboxNode.new('SceneUIVideoImage', root)
--设置节点名字
npcOneVideo.Name = "video"
--设置大小
npcOneVideo.Size = Vector2.new(180, 130)
--设置位置
npcOneVideo.Position = Vector2.new(50, 50)
--设置图片路径
npcOneVideo.Icon = "res/video/login.mp4"
```