# LocalScript(待定)
-----------------------------------------------------------------------------------------
## 描述

`LocalScript`是用于客机运行Lua代码的容器，它作用于仅在客户端的对象，例如玩家的[Camera](/Api/Class/GamePlay/SandboxCameraObject.md)。通过[PlayersRoot](/Api/Class/GamePlay/SandBoxPlayersRoot.md)获得的`LocalPlayer`为当前运行该脚本的玩家

`LocalScript`仅在以下环境下才可运行:

* `Player` 的 `Backpack`，如 `Tool` 的子项

* `Player` 的 `character` 模型

* `Player` 的 `PlayerGui`

* `Player` 的 `PlayerScripts`

* `ReplicatedFirst` 服务

*继承自*：

* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md)


## 代码示例

```lua
print(1)
```