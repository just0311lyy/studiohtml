# SandboxNode Summary

## 节点

- [UI节点 (SceneUIBase)](/#/Api/Class/Scene/SceneUIBase.md)
    - [UI布局组件 (SceneUIComponent)](/#/Api/Class/Scene/SceneUIComponent.md)
        - [按钮组件 (SceneUIButtom)](/#/Api/Class/Scene/SceneUIButtom.md)
        - [图片组件 (SceneUIImage)](/#/Api/Class/Scene/SceneUIImage.md)
        - [video图片 (SceneUIVideoImage)](/#/Api/Class/Scene/SceneUIVideoImage.md)
        - [lable组件 (SceneUITextLabel)](/#/Api/Class/Scene/SceneUITextLabel.md)
        - [输入框组件 (SceneUITextInput)](/#/Api/Class/Scene/SceneUITextInput.md)

    - [UI布局根节点](/#/Api/Class/Scene/SceneUIRoot.md)

- [服务节点](/#/Api/Class/Service/ServiceNode.md)
    - [Game]()
    - [WorkSpace](/#/Api/Class/Scene/SceneRoot.md)
    - [FriendsService](/#/Api/Class/Data/SandboxFriendsService.md)
    - [RunService](/#/Api/Class/Script/RunService.md)
    - [WorldService](/#/Api/Class/GamePlay/SandboxWorldService.md)
    - [UserInputServcie](/#/Api/Class/Animation/UserInputService.md)
    - [ContextActionService](/#/Api/Class/Input/ContextActionService.md)

- 玩法层GAMEPLAY
    - [摄像机](/#/Api/Class/GamePlay/SandboxCameraObject.md)
    - [复活点](/#/Api/Class/GamePlay/SpawnLocation.md)
    - [队伍](/#/Api/Class/GamePlay/SandboxTeam.md)
    - [队伍服务](/#/Api/Class/GamePlay/SandboxTeams.md)
    - [传送服务](/#/Api/Class/GamePlay/SandboxTeleportService.md)
    - [聊天系统](/#/Api/Class/GamePlay/SandboxChat.md)

- 声音SOUND
    - [声音节点](/#/Api/Class/Sound/SandboxSound.md)
    - [声音](/#/Api/Class/Sound/SandboxDefaultSound.md)

- 特效EFEECT
    - [特效](/#/Api/Class/Effect/SandboxDefaultEffect.md)
    - [爆炸](/#/Api/Class/Effect/SandboxExposion.md)
    - [火焰](/#/Api/Class/Effect/SandboxFire.md)
    - [后期效果](/#/Api/Class/Effect/SandboxPostEffectService.md)

- 动画ANIMATIONS
    - [渐变节点](/#/Api/Class/Animation/SceneTweenObject.md)
    - [渐变服务](/#/Api/Class/Animation/SandboxTweenService.md)
    - [动画序列](/#/Api/Class/Animation/SandboxSequenceObject.md)

- [地形节点Terrain](/#/Api/Class/Build/TerrainNode.md)
- [脚本节点](/#/Api/Class/NoType/ScriptNode.md)
    - [主机脚本节点](/#/Api/Class/Script/ScriptObject.md)
    - [客机脚本节点](/#/Api/Class/Script/LocalScriptNode.md)
    - [Module脚本节点](/#/Api/Class/Script/ModuleScriptNode.md)

- [生物节点](/#/Api/Class/Role/SceneActorObject.md)
- [模型节点](/#/Api/Class/Role/SceneModelObject.md)
- 粒子节点
    - [烟雾粒子节点](SandboxParticleSmoke.md)

- [Trans节点](/#/Api/Class/NoType/SceneTransObject.md)
    - [绑点](/#/Api/Class/Bind/SceneBindAttachment.md)
    - [模型容器](/#/Api/Class/Build/SceneModelFolderObject.md)
    - [Primitive](/#/Api/Class/Bind/ScenePrimitiveObject.md)
        - [部件](/#/Api/Class/Build/ScenePartObject.md)

    - [Billboard](/#/Api/Class/Scene/SceneUIBillboard.md)
    - [挂载节点](/#/Api/Class/Bind/SandboxAttachmentObject.md)

- [点击响应](/#/Api/Class/Input/SandboxClickDetectorObject.md)
- [物理关节节点](/#/Api/Class/NoType/SandboxJoint.md)
    - [铰链类型的连接点](/#/Api/Class/Bind/SandboxHingeJoint.md)
    - [固定类型的连接点](/#/Api/Class/Bind/SandboxFixedJoint.md)

- [环境节点](/#/Api/Class/GamePlay/EnvironmentNode.md)
- 组件基类
    - [移动组件基类](BaseLocomotionComponent.md)
    - [BodyComponent](BodyComponent.md)
    - [物理移动组件](PhysXLocoMotionComponent.md)
        - [移动组件](LocoMotionComponent.md)

    - [寻路组件](NavigationPathComponent.md)

- 功能节点
    - 定时器

## 属性类型

- [基础类型]()
    - char,unsigned char,short,unsigned short,int,unsigned int,float,long,unsigned long,long long,unsigned long long,long double,string,bool

- [SandboxNode](/#/Api/Class/NoType/SandboxNode.md)
- [LuaFunction](/#/Api/Parameter/LuaFunction.md)
- [Block](/#/Api/Class/Build/Block.md)
- [Rect](/#/Api/DataType/Rect.md)
- [Ray](/#/Api/DataType/Ray.md)
- [Quaternion](/#/Api/DataType/Quaternion.md)
- [ColourValue](/#/Api/DataType/ColourValue.md)
- 数组
    - [int](/#/Api/DataType/int.md)数组
    - [float](/#/Api/DataType/float.md)数组
    - [ColourValue](/#/Api/DataType/ColourValue.md)数组
    - [SandboxNode](/#/Api/Class/NoType/SandboxNode.md)数组
    - [Vector3](/#/Api/DataType/Vector3.md)数组

- [Vector2](/#/Api/DataType/Vector2.md)
- [Vector3](/#/Api/DataType/Vector3.md)
- [Vector4](/#/Api/DataType/Vector4.md)
- [WCoord](WCoord.md)
- 自定义属性
	- [自定义属性示例]()
	- [Number](long)
	- [Bool](/#/Api/DataType/bool.md)
	- [String](/#/Api/DataType/string.md)
	- [Vector2](/#/Api/DataType/Vector2.md)
	- [Vector3](/#/Api/DataType/Vector3.md)
	- [Vector4](/#/Api/DataType/Vector4.md)
	- [ColourValue](/#/Api/DataType/ColourValue.md)
	- [Rect](/#/Api/DataType/Rect.md)
	- [NumberSequence](vector<float>)
	- [ColourSequence](ColourValue数组)


- [枚举]()
    - [枚举使用]()
    - [BlockPlaceType](/#/Api/Enumerate/UI/BlockPlaceType.md)
    - [TimerRunState](/#/Api/Enumerate/GamePlay/TimerRunState.md)

## 通知

- [自定义通知]()
- [事件通知]()