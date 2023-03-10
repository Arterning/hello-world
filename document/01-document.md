# include <> 和 include "" 的区别

如果你要包含系统库的头文件，应该使用尖括号< >，如果你要包含自己编写的头文件，应该使用双引号" "。

系统库的头文件路径取决于你所使用的编译器和操作系统。

对于Unix/Linux系统来说，通常的标准C库路径为/usr/include，这个路径下包含了大部分的系统库头文件。

# C运行时库

标准C库的源代码通常被称为C运行时库（C runtime library），包含了C语言中的标准函数和数据类型定义等。C运行时库的源代码通常是开放的，但在不同的操作系统和编译器中存放的位置会有所不同。

对于大部分Unix/Linux操作系统，包括常见的Linux发行版，标准C库的源代码通常存放在操作系统的软件包管理系统中，你可以通过相应的包管理器进行下载和安装。标准C库的源代码通常被拆分成多个子模块，每个子模块对应一个源代码包，不同的发行版可能会以不同的方式组织这些包。

如果你希望直接查看标准C库的源代码，可以参考C语言国际标准（ISO/IEC 9899）所定义的C库规范，该规范定义了标准C库中包含的所有函数和数据类型，并提供了相关的实现建议。该规范的最新版本为ISO/IEC 9899:2018，你可以在ISO官网上购买相关的标准文档。

需要注意的是，C运行时库是非常庞大和复杂的，其中包含了大量的系统调用、底层实现细节以及与操作系统紧密相关的代码。在绝大多数情况下，应用程序无需了解C运行时库的具体实现细节，只需要包含相应的头文件即可使用库函数。