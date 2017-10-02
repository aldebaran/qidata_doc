Installation
============

Supported platforms
-------------------

For now, qidata has only been tested on:
 * Ubuntu 14.04
 * Ubuntu 16.04

Using:
 * Python 2.7

Tests on other platforms and with different Python versions are coming, but
might take a while.


Basic installation
------------------

If you want to use qidata through its graphical applications, run::

	pip install qidata_gui

If you only need it to annotate data through Python scripts or to run tests,
you can simply call::

	pip install qidata

And that's it. There is nothing more to do.


Troubleshooting
---------------

Until this day, the only frequent problem I saw was the unability to install
``opencv-python``. This is generally due to a deprecated version of pip.
Upgrading pip to a version higher than 9.0 usually fixes the issue (the default
Ubuntu version is 1.5). Check
`this link <https://pip.pypa.io/en/stable/installing/>`_ to upgrade pip.

If you have any other issue, please report a bug
`here <https://github.com/aldebaran/qidata_doc/issues>`_ with the label
"installation".