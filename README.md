# Python学习笔记

在很久以前，我早就从各大技术群里了解到Python，以及其应用在信息采集方面的强大性能。一年前，机缘巧合下，我人生的第二份工作来到了08cms团队，而接手的第一份工作就是负责汽车系统的汽车信息采集，不过当时只是依葫芦画瓢地使用火车头采集器完成任务。一年后，在我即将离开08cms团队之际，我原计划完成最后一次信息采集任务，与信息采集告一段落。然而，我却碰上了汽车之家的防采集改版，开始了一段各种研究火车头采集器、正则表达式以及防采集方法的煎熬时光。或许，火车头采集器比我想象中强大，但是介于一直以来受前人规则的约束，以及个人爱造轮子的坏习惯，所以我开始了与Python的握手。

## 关于Python

- 不同的编程语言，最后都被“翻译”成CPU可以执行的机器指令。
- Python是一种计算机程序设计语言，是一种相当**高级**的语言。
- Python的定位是“优雅”、“明确”、“简单”。
- 总的来说，Python的哲学就是简单优雅，尽量写容易看明白的代码，尽量写少的代码。
- Python提供了非常完善的基础代码库，覆盖了网络、文件、GUI、数据库、文本等大量内容，被形象地称作“内置电池（batteries included）”。
- Python还有大量的第三方库，也就是别人开发的，供你直接使用的东西。当然，如果你开发的代码通过很好的封装，也可以作为第三方库给别人使用。

![CHALLENGE ACCEPTED!](https://www.liaoxuefeng.com/files/attachments/00138676512923004999ceca5614eb2afc5c0efdd2e4640000/0)

**Python的缺点：**

第一个缺点就是运行速度慢，和C程序相比非常慢，因为Python是解释型语言，你的代码在执行时会一行一行地翻译成CPU能理解的机器码，这个翻译过程非常耗时，所以很慢。而C程序是运行前直接编译成CPU能执行的机器码，所以非常快。

![运行速度慢](https://www.liaoxuefeng.com/files/attachments/001386817301840d023640b45b844b99ab37e34106f2eaa000/0)

第二个缺点就是代码不能加密。如果要发布你的Python程序，实际上就是发布源代码，这一点跟C语言不同，C语言不用发布源代码，只需要把编译后的机器码（也就是你在Windows上常见的xxx.exe文件）发布出去。要从机器码反推出C代码是不可能的，所以，凡是编译型的语言，都没有这个问题，而解释型的语言，则必须把源码发布出去。

![代码不能加密](https://www.liaoxuefeng.com/files/attachments/0013868176293326466225daa824587bef6bb39c8683c2c000/0)

## 安装Python

### 在Windows上安装Python（由于本人暂未win系开发者，请见谅）

首先，根据你的Windows版本（64位还是32位）从Python的官方网站下载Python 3.5对应的64位安装程序或32位安装程序，然后，运行下载的EXE安装包：

![Python安装图示](https://www.liaoxuefeng.com/files/attachments/0014466016166222cc7c2907cef4caab66ad8d53e77841e000/l)

特别要注意勾上`Add Python 3.5 to PATH`，然后点“Install Now”即可完成安装。

运行Python

安装成功后，打开命令提示符窗口，敲入python后，会出现两种情况：

情况一：

![Python安装成功图示](https://www.liaoxuefeng.com/files/attachments/001446601591019cbba6e698d32429bb4754753d86e286a000/l)

看到上面的画面，就说明Python安装成功！

你看到提示符 `>>>` 就表示我们已经在Python交互式环境中了，可以输入任何Python代码，回车后会立刻得到执行结果。现在，输入 `exit()` 并回车，就可以退出Python交互式环境（直接关掉命令行窗口也可以）。

情况二：得到一个错误：

`‘python’ 不是内部或外部命令，也不是可运行的程序或批处理文件。`

![Python安装失败图示](https://www.liaoxuefeng.com/files/attachments/001446601870723ab450ea6b8f946fe841332b542e8f2cc000/l)

这是因为Windows会根据一个 `Path` 的环境变量设定的路径去查找 `python.exe` ，如果没找到，就会报错。如果在安装时漏掉了勾选 `Add Python 3.5 to PATH` ，那就要手动把 `python.exe` 所在的路径添加到 `Path` 中。

如果你不知道怎么修改环境变量，建议把Python安装程序重新运行一遍，务必记得勾上 `Add Python 3.5 to PATH` 。

### Python解释器

当我们编写Python代码时，我们得到的是一个包含Python代码的以 `.py` 为扩展名的文本文件。要运行代码，就需要Python解释器去执行 `.py` 文件。

由于整个Python语言从规范到解释器都是开源的，所以理论上，只要水平够高，任何人都可以编写Python解释器来执行Python代码（当然难度很大）。

事实上，确实存在多种Python解释器,但使用最广泛的还是CPython。如果要和Java或.Net平台交互，最好的办法不是用Jython或IronPython，而是通过网络调用来交互，确保各程序之间的独立性。

**CPython**

当我们从Python官方网站下载并安装好Python 3.5后，我们就直接获得了一个官方版本的解释器：CPython。这个解释器是用C语言开发的，所以叫CPython。在命令行下运行python就是启动CPython解释器。


## 学习教程
[Python教程 - 廖雪峰的官方网站](https://www.liaoxuefeng.com/wiki/0014316089557264a6b348958f449949df42a6d3a2e542c000/ "Python教程 - 廖雪峰的官方网站")
