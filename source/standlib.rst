标准库
=======

.. contents::

Python中的标准库是非常强大的，本章简单介绍一下关于python标准库里面的东西。

dis
---

这个库可以把python字节码转换成类似于汇编语言的东西，比如我定义一个myfunc:

.. code:: python

  def myfunc(alist):
      return len(alist)

然后调用dis，来查看运行的过程::

  >>> dis.dis(myfunc)
    2           0 LOAD_GLOBAL              0 (len)
                3 LOAD_FAST                0 (alist)
                6 CALL_FUNCTION            1
                9 RETURN_VALUE

refer
^^^^^

https://docs.python.org/2/library/dis.html#module-dis

doctest
-------

这个库是用来进行文档测试的，在文档中写出这个方法的使用过程。

调用方法是::

    import doctest
    doctest.testmod()
    
如此一来就可以进行相关的测试

refer
^^^^^^
https://docs.python.org/3/library/doctest.html
