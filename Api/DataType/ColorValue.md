# ColorValue
------------------------------------------------------------------------------------------
## 描述

存储颜色值的变量
注意：构造之后只读，对于实例中的 R/G/B/A 进行修改是无意义的

------------------------------------------------------------------------------------------
## 属性


|<div style="width:1125px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">R</font>]()</div>|
|:---|



|<div style="width:1125px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">G</font>]()</div>|
|:---|



|<div style="width:1125px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">B</font>]()</div>|
|:---|


|<div style="width:1125px">[float](/Api/DataType/Float.md) &emsp;[<font color="dd00dd">A</font>]()</div>|
|:---|


------------------------------------------------------------------------------------------
## 示例代码

```lua
--同ColorQuad的区别是 取值区间是0-1.0f
local color = ColorValue.new(0,0,0,0.0f)

print("color R:"..tostring(color.R).." G:"..tostring(color.G).." B:"..tostring(color.B).." A:"..tostring(color.A))
--color R:0 G:0 B:0 A:0.0f
```