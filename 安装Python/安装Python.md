# 安装Python

## 在Windows上安装Python（由于本人暂未win系开发者，请见谅）

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

## Python解释器

当我们编写Python代码时，我们得到的是一个包含Python代码的以 `.py` 为扩展名的文本文件。要运行代码，就需要Python解释器去执行 `.py` 文件。

由于整个Python语言从规范到解释器都是开源的，所以理论上，只要水平够高，任何人都可以编写Python解释器来执行Python代码（当然难度很大）。

事实上，确实存在多种Python解释器,但使用最广泛的还是CPython。如果要和Java或.Net平台交互，最好的办法不是用Jython或IronPython，而是通过网络调用来交互，确保各程序之间的独立性。

**CPython**

当我们从Python官方网站下载并安装好Python 3.5后，我们就直接获得了一个官方版本的解释器：CPython。这个解释器是用C语言开发的，所以叫CPython。在命令行下运行python就是启动CPython解释器。
