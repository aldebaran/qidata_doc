
Extend possible device list
---------------------------

You might have notice that, in the context, there is a field to describe the
device used to make the dataset. The only problem is that, to select a device as
the dataset's recorder, it needs to be stored in a specific list. The default
one is defined here:

https://github.com/aldebaran/qidata_devices

So, what if your device is not listed ? There are three possibilities:

	1) My device is a public device

	You can edit the list directly on github and make a PR. Once accepted, you
	can either wait for a new package to be generated or directly download and
	install it from source

	2) My device is private but I am the only one needing it

	Same as above except that instead of making a PR, clone the repo, make your
	changes and install your modified version

	3) My device is private, but others, in a private organisation, need it

	You will need to create a new python package, with your device(s) in it.
	You can find a template :download:`here <downloads/qidata_device_template.zip>`.
	Once created, install it::

		python setup.py sdist
		pip install dist/*

	and share the archive in dist/ to your organisation.


Create new annotation messages
------------------------------

Another thing you might have noticed, is that you cannot annotate anything. If
you wish to annotate all trucks in an image, then you need to define a Truck
message somewhere. But where is that ?

Same as above, there are three possibilities, which are very similar. You can
first require to add a message in the `qidata project <https://github.com/aldebaran/qidata>`_
and make a PR, or do the same without the PR, or make your own python package
with your messages that you can share with your organisation.

To create a new annotation message, you can follow the documentation
`here <https://aldebaran.github.io/strong_typing/howtouse.html#create-a-struct>`_,
the only difference being you must replace

::

	from strong_typing import Struct

	class MyStruct(Struct):
		...

by::

	from qidata.metadata_objects import MetadataObject

	class MyStruct(MetadataObject):
		...

You can use :download:`this template <downloads/qidata_new_annotations_template.zip>`
as a starter.