# ModuleScriptNode
------------------------------------------------------------------------------------------
## ������

`ModuleScriptNode`��ֻ������һ�Σ����ұض�������ͬ��һ��ֵ��Ȼ���� `ModuleScriptNode`��ΪΨһ����������£�ͨ������`require`���ش�ֵ������ÿ��`Lua`������`ModuleScriptNode`�����ҽ�����һ�Σ������ں�������`require`ʱ���ظ���ͬ��ֵ��<br>
*�̳���*��

*  [`SandBoxNode`](/Api/Class/SandBoxNode.md)

------------------------------------------------------------------------------------------
## ʾ�����룺

```lua
	local ModuleA = SandboxNode.new("ModuleScriptNode")
	ModuleA.StringCode = "local a = 5 return a+1"

	local value1 = require(ModuleA)
	print("value1:"..value1)
	--value1:6
```