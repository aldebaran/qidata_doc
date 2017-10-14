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

For now, QiData can only be installed by source, and same goes for some of its
dependencies.

Install dependencies
++++++++++++++++++++

First, you need to install xmp::

	git clone https://github.com/aldebaran/xmp.git
	cd xmp
	python setup.py bdist_wheel
	pip install dist/*

Then, you need to install, by similar commands:
 * `image.py <https://github.com/aldebaran/image.py>`_
 * `qidata_devices <https://github.com/aldebaran/qidata_devices>`_

Install qidata
++++++++++++++

First, install qidata main library package::

	git clone https://github.com/aldebaran/qidata.git
	cd qidata
	python setup.py bdist_wheel
	pip install dist/*

Then, if you want to use qidata through its graphical applications, run::

	git clone https://github.com/aldebaran/qidata_gui.git
	cd qidata_gui
	python setup.py bdist_wheel
	pip install dist/*

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