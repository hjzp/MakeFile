寄存器



常见指令

| 指令        | 作用                                                |
| ----------- | --------------------------------------------------- |
| xor a,b     | a异或b                                              |
| test a,b    | 判断a&&b的结果                                      |
| jge         | 有符号数比较判断转移（大于等于）                    |
| jae         | 无符号数比较判断转移（cf=0），前有cmp、test指令调用 |
| lea dst,src | 取src的偏移地址，存入dst                            |