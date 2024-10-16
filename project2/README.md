## CORDIC & Phase Detector

### CODRDIC 
#### Baseline→高效实现
##### 算法 
略
##### 优化
将浮点数类型改为定点数，进而将乘除操作转换为移位操作，提高程序运行效率。

    ap_fixed<W,I> # W表示位宽，I表示整数位宽

位宽和精确度的tradeoff；

### Phase Detector

    fir(I[i],Q[i],&mid_1,&mid_2);
	cordiccart2pol(mid_1,mid_2,&R[i],&Theta[i]);
---
围绕精确度的设计，项目比较简单……

ps:VitisHLS 怎么导出bit文件?(命令行模式下);



