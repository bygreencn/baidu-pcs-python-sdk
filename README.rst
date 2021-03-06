BaiduPCS
========

|Build| |Pypi version| |Pypi downloads|


`百度个人云存储（PCS） <http://developer.baidu.com/ms/pcs>`__ Python SDK

* Documentation: http://baidupcs.rtfd.org
* GitHub: https://github.com/mozillazg/baidu-pcs-python-sdk
* Free software: MIT license
* PyPI: https://pypi.python.org/pypi/baidupcs
* Python version: 2.6, 2.7, 3.3



Installation
------------

To install baidupcs, simply:

.. code-block:: bash

    $ pip install baidupcs


Basic Usage
-----------

.. code-block:: python

    >>> from baidupcs import PCS
    >>> pcs = PCS('access_token')
    >>> response = pcs.info()
    >>> response
    <Response [200]>
    >>> response.ok
    True
    >>> response.status_code
    200
    >>> response.content
    '{"quota":6442450944,"used":5138887,"request_id":1216061570}'
    >>> response.json()
    {u'used': 5138887, u'quota': 6442450944L, u'request_id': 1216061570}


.. |Build| image:: https://api.travis-ci.org/mozillazg/baidu-pcs-python-sdk.png?branch=master
   :target: http://travis-ci.org/mozillazg/baidu-pcs-python-sdk
.. |Pypi version| image:: https://pypip.in/v/baidupcs/badge.png
   :target: https://crate.io/packages/baidupcs
.. |Pypi downloads| image:: https://pypip.in/d/baidupcs/badge.png
   :target: https://crate.io/packages/baidupcs
