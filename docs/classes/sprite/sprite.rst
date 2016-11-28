.. include:: /vars.rst

CSprite
#######

**extends** Vector2_

This page contains documentation on the ``Tga2D::CSprite`` class.
This should be used when you want to draw a sprite to the screen.

Check out the `Rendering a Sprite`_ tutorial.

-----

Constructors
************

Creates a sprite object that can be transformed and rendered to the screen.

.. function:: Tga2D::CSprite(const char* aPath);

* aPath - Specifies the location of the texture for the sprite


Members
*******


myPosition
==========

A Vector2f_ that holds the position of the sprite.

mySize
======

A Vector2f_ that represents the xy-scale of the sprite.



Methods
*******

SetPosition
===========

Moves the sprite to a specified position.

.. function:: void SetPosition( const Tga2D::Vector2f& aVector );

* aVector - The new position of the sprite

.. function:: void SetPosition( float aX, float aY );

* aX - The new x-coordinate of the sprite
* aY - The new y-coordinate of the sprite


Set Size
========

Scales the sprite.

.. function:: void SetSize( const Tga2D::Vector2f& aVector );

* aVector - The new scale of the sprite

.. function:: void SetSize( float aX, float aY);

* aX - The new size of the sprite along the x-axis.
* aY - The new size of the sprite along the y-axis.
