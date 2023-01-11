# PlayFinish
-----------------------------------------------------------------------------------------
## 描述

函数所属类：[SandboxSound](/Api/Class/Sound/SandboxSound.md)

`SandboxSound`实例播放结束时触发该事件

-----------------------------------------------------------------------------------------
## 参数


|<div style="width:200px">名称</div>|<div style="width:200px">类型</div>|<div style="width:200px">默认</div>|<div style="width:200px">描述</div>|
|:--------------------|:--------------------|:--------------------|:--------------------|
|node|[SandboxNode](/Api/Class/NoType/SandboxNode.md)||播放动画的节点|


## 返回

无返回值

------------------------------------------------------------------------------------------
## 示例代码：

```lua
local part = script.Parent --获取父节点
local sound1 = SandboxNode.new('SandboxSound', part) --创建Sound节点
sound1.SoundPath ="sandboxSysId://sounds/npc/chest.ogg" --设置资源路径
sound1.TransObject = script.Parent --绑定TransObject（播放3D声音）
sound1.IsLoop = true --设置循环播放
sound1.PlayOnRemove = true --设置移除时播放
sound1.RollOffMode = Enum.EnumRollOffMode.Linear --设置声音衰减模式
sound1.RollOffMinDistance = 300
sound1.RollOffMaxDistance = 700
sound1:PlaySound() --播放函数

--播放结束事件
sound1.PlayFinish:connect(function(node) 
    node:Destroy()
    print("sound is Destroy")
end)
```