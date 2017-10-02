.. QiData documentation master file

Welcome to QiData's documentation!
==================================

Welcome ! And congratulations you made it here.

But do you know why you are here ? Did you come on purpose, or did you just find
an open door and thought it seemed nice to come in ? Whichever it is, we are
glad to welcome you, and happy to tell you what we do here.

A world of data
---------------

For hundred of purposes, **data** is the key:
 * machine learning
 * algorithm benchmark
 * unit testing
 * functional testing
 * processing pipe design
 * algorithm optimization / parameters tweak
 * sensor caracterization
 * and probably many others...

For all those purposes, having data representing a situation, a problem, a
scenario the program must be able to handle is crucial to the achievement of the
task. And most of the times, *a few* data is simply not enough.

So, what's this 'QiData' about ?
--------------------------------

``QiData`` is a set of tools made to handle *annotated* files and data sets. It
helps to store information about recorded data in order to be used as ground
truth during testing, or as selection criteria for machine learning or
performance statistics.

How is it different from all other annotation tool that can be found ?
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

It is probably not that much different. However, most of those tools were
designed with a very particular area in mind (machine learning for face
detection or OCR, set of recorded speeches for speech recognition, music
database for music classification). We on the other hand, tried our best to be
as generic as possible, as our key goal is to work with robots, which could
encounter many different situations and need many different algorithms.

As a result, ``qidata`` can work with images and video but also with lasers,
sonars or audio. And most important, ``qidata`` is thought to handle multi-modal
data, whereas most annotation tools available cannot handle more than one data
type.

.. note::

   This is actually our core goal. For now, QiData is mostly limited to
   annotation on images.
   But we will do our best to improve it as fast as we can.

Contents
--------

.. toctree::
   :maxdepth: 2
   :numbered:

   install
