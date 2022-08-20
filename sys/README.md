### Comments from Lion's Commemtary on UNIX 6th edition with source code

#### param.h
> 不包含变量声明，但包含许多操作系统常量和参数的定义，以及三个简单数据结构的声明。包含的常量有可调整的变量tunable variables、不应修改的优先级priorities、信号量signals、不能改变的基础常量、使用字节访问整数的结构体、访问整数的结构体、及某些处理器寄存器。

#### systm.h
> 包含结构`callout`, `mount`的完整声明和定义。注意：这些变量并没有被显示的初始化，因此所有变量都被初始化为0。前三个数组声明均用到了`param.h`中的常数作为参数，因此任何包含`systm.h`的文件之前要包含`param.h`

#### seg.h
> 包含可用来引用段寄存器的一些定义和一个声明。该文件可无损失地被`param.h`和`system.h`文件吸收。

#### proc.h
