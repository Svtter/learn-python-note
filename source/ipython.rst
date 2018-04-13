IPython使用技巧
================

.. contents::


使用IPython查看当前变量
------------------------


This might help you, though it's not exactly what Spyder offers and is much simpler:

To get a list of all currently defined variables, run who :

.. code:: ipython

    In [1]: foo = 'bar'

    In [2]: who
    foo

For more detail, run whos:

.. code:: ipython

    In [3]: whos
    Variable   Type    Data/Info
    ----------------------------
    foo        str     bar

For a complete list of built-in functions see Magic Commands

refer
^^^^^

https://stackoverflow.com/questions/37718907/variable-explorer-in-jupyter-notebook/37719560#37719560?newreg=76a86d7a8bc2410998416d13eaf5cf08
