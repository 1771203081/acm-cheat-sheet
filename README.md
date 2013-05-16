#手写代码必备手册
-----------------

C++ 文件夹下是C++版，内容一摸一样，代码是用C++写的，**下载**：[手写代码必备手册(C++版).pdf](https://github.com/soulmachine/acm-cheat-sheet/blob/master/C++/%E6%89%8B%E5%86%99%E4%BB%A3%E7%A0%81%E5%BF%85%E5%A4%87%E6%89%8B%E5%86%8C(C++%E7%89%88).pdf?raw=true)

Java 文件夹下是Java版，内容一摸一样，代码是用Java写的

##LaTeX模板
本书使用的是陈硕开源的[模板](https://github.com/chenshuo/typeset)。该模板已经用于陈硕写的书[《Linux 多线程服务端编程：使用 muduo C++ 网络库》](http://chenshuo.com/book/)，已经出版。

这个模板制作精良，很有taste，感谢陈硕 :)

##在Windows下编译
1. 安装Tex Live 2012 <http://www.tug.org/texlive/>。把bin目录例如`D:\texlive\2012\bin\win32`加入PATH环境变量。
2. 安装TeXstudio <http://texstudio.sourceforge.net/>
3. (可选)启动Tex Live Manager，更新所有已安装的软件包。
4. 安装字体。在Windows下，这个LaTex模板额外使用了5个字体，下载地址 <http://weibo.com/1663402687/zrSNhgTGK>
5. 配置TeXstudio。

    启动Texstudio，选择 `Options-->Configure Texstudio-->Commands`，XeLaTex 设置为 `xelatex -synctex=1 -interaction=nonstopmode %.tex`；

    选择 `Options-->Configure Texstudio-->Build`

    Build & View 由默认的 PDF Chain 改为 Compile & View；

    Default Compiler 由默认的PdfLaTex 修改为 XeLaTex ；

    PDF Viewer 改为 “Internal PDF Viewer(windowed)”，这样预览时会弹出一个独立的窗口，这样比较方便。

6. 编译。用TeXstudio打开`ACM-cheat-sheet.tex`，点击界面上的绿色箭头就可以开始编译了。

    在下方的窗口可以看到TeXstudio正在使用的编译命令是`xelatex -synctex=1 -interaction=nonstopmode "ACM-cheat-sheet".tex`

##如何贡献代码
编译通过后，就具备了完整的LaTeX编译环境了。

本书模板已经写好了，基本上不需要很多LaTeX知识就可以动手了。

欢迎给本书添加内容或纠正错误，在自己本地编译成PDF，预览没问题后，就可以发pull request过来了。