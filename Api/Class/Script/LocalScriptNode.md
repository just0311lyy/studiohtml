# LocalScript(待定)
-----------------------------------------------------------------------------------------
## 描述

[`LocalScript`](/Api/Class/Script/LocalScriptNode.md)是用于客机运行Lua代码的容器，它作用于仅在客户端的对象，例如玩家的[Camera](/Api/Class/GamePlay/SandboxCameraObject.md)。通过[PlayersRoot](/Api/Class/GamePlay/SandBoxPlayersRoot.md)获得的[`LocalPlayer`](/Api/Class/GamePlay/SandBoxLocalPlayer.md)为当前运行该脚本的玩家

[`LocalScript`](/Api/Class/Script/LocalScriptNode.md)仅在以下环境下才可运行:

* [`Player`](/Api/Class/GamePlay/ScenePlayerObject.md) 的 [`Backpack`](/Api/Class/GamePlay/SandboxBackpack.md)，如 [`Tool`](/Api/Class/GamePlay/SandboxTool.md) 的子项

* [`Player`](/Api/Class/GamePlay/ScenePlayerObject.md) 的 `character` 模型

* [`Player`](/Api/Class/GamePlay/ScenePlayerObject.md) 的 `PlayerGui`

* [`Player`](/Api/Class/GamePlay/ScenePlayerObject.md) 的 `PlayerScripts`

* `ReplicatedFirst` 服务

*继承自*：

* [SandBoxNode](/Api/Class/NoType/SandBoxNode.md)


## 代码示例

```lua
print(1)
```