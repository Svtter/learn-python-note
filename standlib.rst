标准库
=======

Python中的标准库是非常强大的，本章简单介绍一下关于python标准库里面的东西。

dis
---

这个库可以把python字节码转换成类似于汇编语言的东西，比如我定义一个myfunc::

  def myfunc(alist):
      return len(alist)

然后调用dis，来查看运行的过程::

  >>> dis.dis(myfunc)
    2           0 LOAD_GLOBAL              0 (len)
                3 LOAD_FAST                0 (alist)
                6 CALL_FUNCTION            1
                9 RETURN_VALUE
