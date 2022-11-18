# AreaNode
------------------------------------------------------------------------------------------
## ����

�̳У�`SandboxNode`

------------------------------------------------------------------------------------------
## ����

|<div style="width:1125px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">Beg</font>]()</div>|
|:---|
|��ʼλ����������|

|<div style="width:1125px">[Vector3](/Api/DataType/Vector3.md) &emsp;[<font color="dd00dd">End</font>]()</div>|
|:---|
|����λ����������|

|<div style="width:1125px">[int](/Api/DataType/Int.md) &emsp;[<font color="dd00dd">EffectWidth</font>]()</div>|
|:---|
|Ч�����|

|<div style="width:1125px">[bool](/Api/DataType/Bool.md) &emsp;[<font color="dd00dd">Show</font>]()</div>|
|:---|
|�Ƿ���ʾ|

|<div style="width:1125px">[SHOWMODE]() &emsp;[<font color="dd00dd">ShowMode</font>]()</div>|
|:---|
|��ʾģʽ��ö��(`SceneEffectFrame::SHOWMODE`):<br>X = 1,<br>Y = 2,<br>Z = 4,<br>XY = 1+2,<br>XZ = 1+4,<br>YZ = 2+4,<br>XYZ = 1+2+4|


|<div style="width:1125px">[ColorValue](/Api/DataType/ColourValue.md) &emsp;[<font color="dd00dd">Color</font>]()</div>|
|:---|
|����������ɫ|

------------------------------------------------------------------------------------------
## �¼�

|<div style="width:500px">[SBXSignal\<SandboxNode\>]() &emsp;[<font color="dd00dd">NotifyEnterNode</font> ]() ()</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|�ڵ���������||||
|**��������**|||**��Ҫ**|
|SBXSignal|||����ڵ�ʱ�������¼�����Ϊ��`SandboxNode node`��|
|**SBXSignal��������**|**���**|**Ĭ��**|**����**|
|node|SandboxNode||����������`SandboxNode`�ڵ�|

|<div style="width:500px">[SBXSignal\<SandboxNode\>]() &emsp;[<font color="dd00dd">NotifyLeaveNode</font> ]() ()</div>|<div style="width:100px"></div>|<div style="width:45px"></div>|<div style="width:400px"></div>|
|:---|:---|:---|:---|
|�ڵ��뿪������||||
|**��������**|||**��Ҫ**|
|SBXSignal|||�뿪�ڵ�ʱ�������¼�����Ϊ��`SandboxNode node`��|
|**SBXSignal��������**|**���**|**Ĭ��**|**����**|
|node|SandboxNode||�뿪�������`SandboxNode`�ڵ�|

------------------------------------------------------------------------------------------
## ʾ�����룺

```lua
local part = script.Parent --��ȡ���ڵ�
local area = SandboxNode.new('AreaNode', part) --����AreaNode�ڵ�

--����Actorʵ��
local actorNode = SandboxNode.new('SceneActorObject')
actorNode.Name = "my_actor"

--actorNode��������
area.NotifyEnterNode:connect(function(actorNode) 
    print("actorNode��������")
end)
```