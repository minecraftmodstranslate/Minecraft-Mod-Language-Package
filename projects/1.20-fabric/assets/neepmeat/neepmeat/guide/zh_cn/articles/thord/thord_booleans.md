---
id: thord_booleans
---
# 布尔值

THORD没有布尔值类型，不过所有非0值均视为true。

true的标准值为-1。所有比较操作均会将其作为真值返回。

由于整数补码的实际存储特征，各位取反（NEEPASM中为`NOT`，THORD中为`INVERT`）可将-1和0相互转换。


```
-1 invert . # becomes 0 [1]

0 invert . # becomes -1 [2]
```
 [1] 变为0
 [2] 变为-1

将其他非零数各位取反，所得的值不会为零。也即，布尔逻辑只在-1和0这两个值上维持原有功能。
