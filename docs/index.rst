Welcome to TGA2D Documentation!
###############################

Intruduction
************

Hello and welcome to the wonderful world of 2D graphics!
This engine is created for the purpose of having easy access to advanced rendering techniques.
The engine is created in house meaning that most of the teachers here at TGA will have knowledge of it and can always be of assistance.
The engine will be updated the more we use it and with newer tech comming.


What is a 2D engine?
====================

A 2D engine is a framework where the developer can use interfaces and simple techniques without the knowledge of how the underlying tech works.
To load an image and draw it on the screen is a complicated process and will take many hours to get right.
An engine will have this functionality already written, and exposes simple functions.
There are a lot of 2D engines created: https://en.wikipedia.org/wiki/List_of_game_engines
So why not use one of them?
The simple answer is that with our own engine, we have full control and can develop it further to suit this education.
If problems would appear, we can handle it here instead of writing to the creator of the 3rd party engine.


Engine specs
============

DirectX 11

Supports out of the box:

* Text
* Sprites
* Sprite batches
* Video (w/o sound)
* Lights
* Line drawing
* Custom drawing


Good to know
============

This engine operates in a normalized space, meaning nothing is in pixel space.
The top-left corner of the window is position ``{x:0, y:0}``.
The bottom-right corner of the window is position ``{x:1, y:1}``.
You can still set positions outside of these, but then you'll need to move the "camera" to be able to see it.
Colors are also in the normalized space ``0.0 -> 1.0``.
You have the full source! Don't be afraid to get your hands dirty!

Keep it within The Game Assembly please.
We want to support you here 100% at school with it.
That does not mean you can take it home and on other computers.
If you have improvements, please tell us!

Compatible operating systems: Windows 7, Windows 8.X, Windows 10


License
=======

As this engine is developed here at The Game Assembly, you can not create and sell a product with TGA2D. (aka. Free for non commercial use).
If you are looking for an engine to release your own games with we recommend looking at SDL.


.. note:: note

.. tip:: tip

.. attention:: attention

.. caution:: caution

.. danger:: danger

.. error:: error

.. hint:: hint

.. important:: important

.. admonition:: generic admonition


.. warning:: This is not even close to finished, if you feel like something's missing, then click that "Edit on GitHub" button at the top right to contribute!


.. toctree::
	:glob:
	:caption: General
	:maxdepth: 1

	faq


.. toctree::
	:glob:
	:caption: Tutorials
	:maxdepth: 1

	./tutorials/*

.. toctree::
	:glob:
	:caption: Classes
	:maxdepth: 2

	./classes/*

.. toctree::
	:glob:
	:caption: Structs
	:maxdepth: 1

	./structs/*

