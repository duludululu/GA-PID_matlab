GA文件夹是单参数的优化，没考虑负值。若是两三个参数可以把注释掉的内容取消注释即可
GA-PID是优化pid三个参数的遗传算法，其中适应度值的计算考虑了超调、调节时间和误差积分。 theta.slx是对应的模型
遗传算法主要原则：优胜劣汰。
1.初始化
2.适应度计算
3.复制。选择父代中适应值最好的若干保持不变，直接完整的复制到子代中。
4.选择、交叉。通过轮盘赌法选择父代进行交叉
5.变异
编码采用2进制，考虑保留4位小数，因此根据上下限之间的范围，如[0,9],   (9-0)*10000  然后求出对应的需要的二进制的位数 =17
