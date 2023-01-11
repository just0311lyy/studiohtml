<!-- 注：
本地调试路径 /#/Api/Class/Scene/SceneUIBase.md
线上跳转路径 /studiohtml/#/Api/Class/Scene/SceneUIBase.md -->

# SandboxNode Summary

## Node

- [UIBase](/#/Api/Class/Scene/SceneUIBase.md)
    - [UIComponent](/#/Api/Class/Scene/SceneUIComponent.md)
        - [UIButtom](/#/Api/Class/Scene/SceneUIButtom.md)
        - [UIImage](/#/Api/Class/Scene/SceneUIImage.md)
        - [UIVideoImage](/#/Api/Class/Scene/SceneUIVideoImage.md)
        - [UITextLabel](/#/Api/Class/Scene/SceneUITextLabel.md)
        - [UITextInput](/#/Api/Class/Scene/SceneUITextInput.md)

    - [UIRoot](/#/Api/Class/Scene/SandboxUIRoot.md)

- [Service](/#/Api/Class/Service/ServiceNode.md)
    - Game
    - [WorkSpace](/#/Api/Class/Scene/SceneRoot.md)
    - [FriendsService](/#/Api/Class/Data/SandboxFriendsService.md)
    - [RunService](/#/Api/Class/Script/RunService.md)
    - [WorldService](/#/Api/Class/GamePlay/SandboxWorldService.md)
    - [UserInputServcie](/#/Api/Class/Animation/UserInputService.md)
    - [ContextActionService](/#/Api/Class/Input/ContextActionService.md)

- GAMEPLAY
    - [Camera](/#/Api/Class/GamePlay/SandboxCameraObject.md)
    - [SpawnLocation](/#/Api/Class/GamePlay/SpawnLocation.md)
    - [Team](/#/Api/Class/GamePlay/SandboxTeam.md)
    - [Teams](/#/Api/Class/GamePlay/SandboxTeams.md)
    - [TeleportService](/#/Api/Class/GamePlay/SandboxTeleportService.md)
    - [Chat](/#/Api/Class/GamePlay/SandboxChat.md)

- SOUND
    - [Sound](/#/Api/Class/Sound/SandboxSound.md)
    - [DefaultSound](/#/Api/Class/Sound/SandboxDefaultSound.md)

- EFEECT
    - [DefaultEffect](/#/Api/Class/Effect/SandboxDefaultEffect.md)
    - [Exposion](/#/Api/Class/Effect/SandboxExposion.md)
    - [Fire](/#/Api/Class/Effect/SandboxFire.md)
    - [PostEffectService](/#/Api/Class/Effect/SandboxPostEffectService.md)

- ANIMATIONS
    - [UITween](/#/Api/Class/Animation/SceneTweenObject.md)
    - [TweenService](/#/Api/Class/Animation/SandboxTweenService.md)
    - [Sequence](/#/Api/Class/Animation/SandboxSequenceObject.md)
    - [AnimationAsset](/#/Api/Class/Animation/SandboxAnimationAsset.md)
    - [AnimatorBase](/#/Api/Class/Animation/SandboxAnimatorBase.md)
    - [Animation](/#/Api/Class/Animation/SandboxAnimation.md)
    - [AttributeAnimation](/#/Api/Class/Animation/SandboxAttributeAnimation.md)
    - [AnimatorLayer](/#/Api/Class/Animation/SandboxAnimatorLayer.md)
    - [AnimatorLayerData](/#/Api/Class/Animation/SandboxAnimatorLayerData.md)
    - [AnimatorStateData](/#/Api/Class/Animation/SandboxAnimatorStateData.md)
    - [AnimatorStateMachineData](/#/Api/Class/Animation/SandboxAnimatorStateMachineData.md)
    - [AnimatorController](/#/Api/Class/Animation/SandboxAnimatorController.md)
    - [Animator](/#/Api/Class/Animation/SandboxAnimator.md)

- [Terrain](/#/Api/Class/Build/TerrainNode.md)
    - [BluePrint](/#/Api/Class/Build/SandboxBluePrint.md)
    - [Decal](/#/Api/Class/Scene/SandboxDecalObject.md)
    - [GeoSolid](/#/Api/Class/Build/SceneGeoSolid.md)
    - [Light](/#/Api/Class/Build/SandboxLightObject.md)
    - [Material](/#/Api/Class/Script/SandboxMaterialObject.md)
    - [Voxel](/#/Api/Class/GamePlay/SandboxVoxelObject.md)

- [ScriptNode](/#/Api/Class/NoType/ScriptNode.md)
    - [Script](/#/Api/Class/Script/ScriptObject.md)
    - [LocalScript](/#/Api/Class/Script/LocalScriptNode.md)
    - [ModuleScript](/#/Api/Class/Script/ModuleScriptNode.md)

- ROLE
    - [Actor](/#/Api/Class/Role/SceneActorObject.md)
    - [Model](/#/Api/Class/Role/SceneModelObject.md)
    - [AIBase](/#/Api/Class/Role/SandboxAIBase.md)
    - [AITaskEntry](/#/Api/Class/Role/SandboxAITaskEntry.md)

- PARTICLE
    - [ParticleSmoke](/#/Api/Class/Effect/SandboxParticleSmoke.md)

- [Transform](/#/Api/Class/NoType/SceneTransObject.md)
    - [BindAttachment](/#/Api/Class/Bind/SceneBindAttachment.md)
    - [UIModelFolder](/#/Api/Class/Build/SceneModelFolderObject.md)
    - [UIBillboard](/#/Api/Class/Scene/SceneUIBillboard.md)
    - [Attachment](/#/Api/Class/Bind/SandboxAttachmentObject.md)

- [ClickDetector](/#/Api/Class/Input/SandboxClickDetectorObject.md)
- [Joint](/#/Api/Class/NoType/SandboxJoint.md)
    - [HingeJoint](/#/Api/Class/Bind/SandboxHingeJoint.md)
    - [FixedJoint](/#/Api/Class/Bind/SandboxFixedJoint.md)

- [Environment](/#/Api/Class/GamePlay/EnvironmentNode.md)
- COMPONENT
    - BodyComponent
    - PhysXLocoMotionComponent
        - LocoMotionComponent

    - NavigationPathComponent

- FUNCTION
    - [Timer](/#/Api/Class/Script/TimerNode.md)

## DATA TYPE

- Number
- [Int](/#/Api/DataType/Int.md)
- [Bool](/#/Api/DataType/Bool.md)
- [String](/#/Api/DataType/String.md)

- [SandboxNode](/#/Api/Class/NoType/SandboxNode.md)
- [LuaFunction](/#/Api/Parameter/LuaFunction.md)
- [Block](/#/Api/Class/Build/Block.md)
- [Rect](/#/Api/DataType/Rect.md)
- [Ray](/#/Api/DataType/Ray.md)
- [Quaternion](/#/Api/DataType/Quaternion.md)
- [colorValue](/#/Api/DataType/colorValue.md)
- ReflexTuple
    - ReflexTuple([int](/#/Api/DataType/int.md))
    - ReflexTuple([float](/#/Api/DataType/float.md))
    - ReflexTuple([colorValue](/#/Api/DataType/colorValue.md))
    - ReflexTuple([SandboxNode](/#/Api/Class/NoType/SandboxNode.md))
    - ReflexTuple([Vector3](/#/Api/DataType/Vector3.md))

- [Vector2](/#/Api/DataType/Vector2.md)
- [Vector3](/#/Api/DataType/Vector3.md)
- [Vector4](/#/Api/DataType/Vector4.md)
- [WCoord](WCoord.md)

- CUSTOM ATTRIBUTES
	- Number
	- [Bool](/#/Api/DataType/Bool.md)
	- [String](/#/Api/DataType/String.md)
	- [Vector2](/#/Api/DataType/Vector2.md)
	- [Vector3](/#/Api/DataType/Vector3.md)
	- [Vector4](/#/Api/DataType/Vector4.md)
	- [Color](/#/Api/DataType/colorValue.md)
	- [Rect](/#/Api/DataType/Rect.md)
	- NumberSequence
	- colorSequence

- EUNMERATE

    - [DefaultSound](/#/Api/Enumerate/Sound/EnumDefaultSound.md)
    - [ListenerType](/#/Api/Enumerate/Sound/EnumListenerType.md)
    - [RollOffMode](/#/Api/Enumerate/Sound/EnumRollOffMode.md)
    - [DefaultEffect](/#/Api/Enumerate/Effect/EnumDefaultEffect.md)
    - [ExplosionType](/#/Api/Enumerate/Effect/ExplosionType.md)
    - [AutoSizeType](/#/Api/Enumerate/UI/AutoSizeType.md)
    - [BLOCKPLACETYPE](/#/Api/Enumerate/UI/BLOCKPLACETYPE.md)
    - [ButtonDownEffect](/#/Api/Enumerate/UI/ButtonDownEffect.md)
    - [EasingDirection](/#/Api/Enumerate/UI/EasingDirection.md)
    - [EasingStyle](/#/Api/Enumerate/UI/EasingStyle.md)
    - [FillMethod](/#/Api/Enumerate/UI/EnumFillMethod.md)
    - [FillOrigin](/#/Api/Enumerate/UI/EnumFillOrigin.md)
    - [LayoutHRelation](/#/Api/Enumerate/UI/EnumLayoutHRelation.md)
    - [LayoutVRelation](/#/Api/Enumerate/UI/EnumLayoutVRelation.md)
    - [LayoutSizeRelation](/#/Api/Enumerate/UI/EnumLayoutSizeRelation.md)
    - [InputMode](/#/Api/Enumerate/UI/InputMode.md)
    - [ListLayoutType](/#/Api/Enumerate/UI/ListLayoutType.md)
    - [MouseBehavior](/#/Api/Enumerate/UI/MouseBehaviorEnum.md)
    - [OverflowType](/#/Api/Enumerate/UI/OverflowType.md)
    - [RenderPriority](/#/Api/Enumerate/UI/RenderPriority.md)
    - [TextHAlignment](/#/Api/Enumerate/UI/TextHAlignment.md)
    - [TextVAlignment](/#/Api/Enumerate/UI/TextVAlignment.md)
    - [TweenStatus](/#/Api/Enumerate/UI/TweenStatus.md)
    - [Weather](/#/Api/Enumerate/GamePlay/EnumWeather.md)
    - [SkyPlanet](/#/Api/Enumerate/GamePlay/EnumSkyPlanet.md)
    - [TimerRunState](/#/Api/Enumerate/GamePlay/TimerRunState.md)
    - [Action](/#/Api/Enumerate/UserInput/Action.md)
    - [ContextActionPriority](/#/Api/Enumerate/UserInput/ContextActionPriority.md)
    - [ContextActionResult](/#/Api/Enumerate/UserInput/ContextActionResult.md)
    - [ContextActionType](/#/Api/Enumerate/UserInput/ContextActionType.md)
    - [UserInputState](/#/Api/Enumerate/UserInput/UserInputState.md)
    - [UserInputType](/#/Api/Enumerate/UserInput/UserInputType.md)
    - [KeyCode](/#/Api/Enumerate/UserInput/KeyCode.md)
## NOTIFY

- CustomNotify
- ReflexClassNotify