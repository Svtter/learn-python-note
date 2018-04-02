======================
解决python2-3的兼容问题
======================

.. contents::

six
----

解决Python2-3的兼容问题，可以使用 ``six`` 来做许多工作。

.. code:: python
  from six.moves import urllib
  # import urllib.request


如此以来，可以替换 ``urllib``

__future__
^^^^^^^^^^^

在 ``__init__`` 包中引入 ``from __future__ import division`` 可以将python2中的除法变为python3
