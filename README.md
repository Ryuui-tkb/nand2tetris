# Build a Modern Computer from First Principles: From Nand to Tetris(nand2tetris)

## 前言


2021年5月，我顺利从原东家跳槽到现在的公司。正值新冠疫情时期，入职的第二天开始，我就开启了work at home模式。因此，节约了耗费在工作之外的通勤时间，可以用来课外的学习时间。7月，在完成了前一个算法方面的课程之后，我思考着接下来要进行的项目。

一直以来，我都意识到自己对计算机系统的整体框架不甚了解。尤其是硬件的部分，知识储备一直停留在大学课本的理论上，所以我找到了这门从与非门开始构建计算机，并且最后实现软件运行的课程。通过学习和实战，我发现这是一门很有价值的课程，于是希望能分享给其他小伙伴一起学习。

本项目始于2021年8月, 向github迁移的工作开始于2021年10月。   
截至写下前言的时候，我已经基本完成该项目的前半部分，即硬件的构建部分。至于后面的软件部分，我将在完成手头另一个算法课程后继续更新，预计在11月后旬开始。

欢迎各位一起学习，多多指教。

## 简介
(摘自[Coursera官方课程](https://www.coursera.org/learn/build-a-computer))
>What you’ll achieve:   
In this project-centered course* you will build a modern computer system, from the ground up. We’ll divide this fascinating journey into six hands-on projects that will take you from constructing elementary logic gates all the way through creating a fully functioning general purpose computer. In the process, you will learn - in the most direct and constructive way - how computers work, and how they are designed.   
What you’ll need:   
This is a self-contained course: all the knowledge necessary to succeed in the course and build the computer system will be given as part of the learning experience. Therefore, we assume no previous computer science or engineering knowledge, and all learners are welcome aboard. You will need no physical materials, since you will build the computer on your own PC, using a software-based hardware simulator, just like real computers are designed by computer engineers in the field. The hardware simulator, as well as other software tools, will be supplied freely after you enroll in the course.   
Course format:   
The course consists of six modules, each comprising a series of video lectures, and a project. You will need about 2-3 hours to watch each module's lectures, and about 5-10 hours to complete each one of the six projects. The course can be completed in six weeks, but you are welcome to take it at your own pace. You can watch a TED talk about this course by Googling "nand2tetris TED talk".

简而言之，该项目面对掌握任意一门编程语言的小伙伴。

通过这个项目，可以获得以下技能：

* 大致熟悉计算机自相而上的整体框架
* 在硬件模拟器上构建一台计算机，并运行软件

## 书籍

* [**中文版(已绝版)**](https://book.douban.com/subject/1998341/): Noam Nisan, Shimon Schocken.计算机系统要素：从零开始构建现代计算机[M].电子工业出版社, 2007.
* [**日本語版**](https://www.oreilly.co.jp/books/9784873117126/): Noam Nisan, Shimon Schocken.コンピュータシステムの理論と実装 ―モダンなコンピュータの作り方[M].オライリージャパン, 2015.
* [**English Edition**](https://mitpress.mit.edu/books/elements-computing-systems-second-edition): Noam Nisan, Shimon Schocken.The Elements of Computing Systems, second edition: Building a Modern Computer from First Principles[M].The MIT Press, 2021.


## 其他参考资料
* [Coursera课程](https://www.coursera.org/learn/build-a-computer)
* [官方网站](https://www.nand2tetris.org) 
* [开发套件下载及使用说明](https://www.nand2tetris.org/software) 


## 项目大纲

本项目依据Coursera上的官方课程，将项目分为2部分。

* [1. Build a Modern Computer from First Principles: From Nand to Tetris](https://www.coursera.org/learn/build-a-computer)
* [2. Build a Modern Computer from First Principles: Nand to Tetris Part II](https://www.coursera.org/learn/nand2tetris2) 

全项目共计13章。其中：   
Part1为6章，着重于硬件层的构建，并且在最后一单元会涉及软件层的汇编编译器构建。   
Part2分为7章，着重于软件层的构建。

各章内容如下。

1.[**布尔逻辑**](projects/01/README.md): 各类基础逻辑门，基于nand门实现。

* 与门[And], 16位与门[And16]
* 或门[Or], 16位或门[Or16], 8通道或门[Or8Way]
* 非门[Not], 16位非门[Not16]
* 异或门[Xor]
* 复用器[Mux], 16位复用器[Mux16], 4通道16位复用器[Mux4Way16], 8通道16位复用器[Mux8Way16]
* 解复用器[DMux], 4通道解复用器[DMux4Way], 8通道解复用器[DMux8Way]

2.[**布尔运算**](projects/02/README.md): 布尔运算的基础知识，实现了加法器和运算逻辑单元(ALU)。

* 16位二进制加法[Add16]
* 半加器[HalfAdder]
* 全加器[FullAdder]
* 增量器[inc16]
* 运算逻辑单元[ALU]

## 常见问题
* [macOS下, 使用'.sh'文件打开'.bat'文件时，无权限错误]()
## License
MIT