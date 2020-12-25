# proj24-rt-smart-porting
### 项目描述

目前在RISC-V平台的OS还较少，支持MMU的OS也比较少，因此本项目以支持MMU虚拟内存机制的RT-Thread Smart（简称rt-smart）为基础，在qemu上以及K210上实现运行。

### 所属赛道

2021全国大学生操作系统比赛的“OS功能设计”赛道



### 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2021年春季学期或之后本科毕业的大一~大四的学生）
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“2021全国大学生操作系统比赛”的章程和技术方案要求



### 项目导师

**熊谱翔**

* github [BernardXiong](https://github.com/BernardXiong)

* email bernard.xiong@rt-thread.com



### 难度

中等



### 特征

* 系统调用接口支持POSIX子集，

* 采用musl libc

* 支持RISC-V平台

* rt-smart支持qemu仿真与Kendryte K210（含MMU和S模式）



### License

* [Apache-2.0](https://opensource.org/licenses/Apache-2.0)



## 预期目标

### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标

### 第一题：rt-smart在qemu上的移植

该移植只需要适配qemu的uart与timer硬件，同时完成musl libc库相关接口的对接。

### 第二题：rt-smart在K210平台上的基础移植

该移植需要适配qemu的uart与timer硬件，实现MMU的对接，保证系统运行在S态，用户程序运行在U态，并能正常运行相关测试程序。

### 第三题（可选）：rt-smart在K210平台上的硬件和功能适配

该题目可以选择适配gpio、spi等驱动，实现spi flash读写，实现多串口支持，实现可读写文件系统的挂载，实现可读写文件系统分区的用户程序下载。