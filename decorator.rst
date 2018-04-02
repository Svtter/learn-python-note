装饰器
======

.. contents::
  

装饰器的本质是什么？
-----------------

Remember, that the @decorator syntax is just syntactic sugar; the syntax:

.. code:: python

  @property
  def foo(self): return self._foo


really means the same thing as


.. code:: python

  def foo(self): return self._foo
  foo = property(foo)
