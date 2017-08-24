# 第一个Python程序

![Hello world](https://www.liaoxuefeng.com/files/attachments/001431639811536fb2d4d2944694d419486215f55c8d544000/l)

在交互式环境的提示符 `>>>` 下，直接输入代码，按回车，就可以立刻得到代码执行结果。

任何有效的数学计算都可以算出来。

`>>> 100+200`

`300`

如果要让Python打印出指定的文字，可以用print()函数，然后把希望打印的文字用单引号或者双引号括起来，但不能混用单引号和双引号：

```
>>>print('hello, world')
hello, world
```

这种用单引号或者双引号括起来的文本在程序中叫字符串。

最后，用 `exit()` 退出Python。


**命令行模式和Python交互模式**

请注意区分命令行模式和Python交互模式。

看到类似 `C:\>` 是在Windows提供的命令行模式：

![Windows提供的命令行模式](https://www.liaoxuefeng.com/files/attachments/0014466032359027375f5bf19fc4fee81b8247d1ecb47a9000/l)

在命令行模式下，可以执行 `python` 进入Python交互式环境，也可以执行 `python hello.py` 运行一个 `.py` 文件。

看到 `>>>` 是在Python交互式环境下：

![Python交互式环境](https://www.liaoxuefeng.com/files/attachments/001446601591019cbba6e698d32429bb4754753d86e286a000/l)

在Python交互式环境下，只能输入Python代码并立刻执行。

此外，在命令行模式运行 `.py` 文件和在Python交互式环境下直接运行Python代码有所不同。Python交互式环境会把每一行Python代码的结果自动打印出来，但是，直接运行Python代码却不会。

例如，在Python交互式环境下，输入：

```
>>> 100 + 200 + 300
600
```

直接可以看到结果 `600` 。

但是，写一个 `calc.py` 的文件，内容如下：

```
100 + 200 + 300
```

然后在命令行模式下执行：

```
C:\work>python calc.py
```

发现什么输出都没有。

这是正常的。想要输出结果，必须自己用 `print()` 打印出来。把 `calc.py` 改造一下：

```
print(100 + 200 + 300)
```

再执行，就可以看到结果：

```
C:\work>python calc.py
600
```
