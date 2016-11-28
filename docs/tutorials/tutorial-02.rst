Rendering a Sprite
===================

We have skipped out on most of the image formats supported to give you a good ground on how to create and load textures(actual images).
The engine craves the image format `.dds`_.
This image format is good in a number of ways when dealing with game engine textures.
The image can be saved with `mip maps`_ (useful later in 3D), and is enforced to be in a resolution of power of 2 which is optimised in shaders and will generate a higher frame rate.

.. _.dds: https://en.wikipedia.org/wiki/DirectDraw_Surface
.. _mip maps: https://en.wikipedia.org/wiki/Mipmap


The fun stuff
^^^^^^^^^^^^^^^^^^^

Lets render an image!
The only thing we need to do is create an instance of the class ``Tga2D::CSprite``.

.. code-block:: cpp
	:caption: GameWorld.h
	:name: gameworld_h
	:linenos:
	:emphasize-lines: 5,17

	#pragma once

	namespace Tga2D
	{
		class CSprite;
	}

	class CGameWorld
	{
	public:
		CGameWorld();
		~CGameWorld();
		void Init();
		void Update(float aTimeDelta);

	private:
		Tga2D::CSprite* mySprite;
	};

.. code-block:: cpp
	:caption: GameWorld.cpp
	:name: gameworld_cpp
	:linenos:
	:emphasize-lines: 3,7,13

	#include "stdafx.h"
	#include "GameWorld.h"
	#include <tga2d/sprite/sprite.h>

	void CGameWorld::Init()
	{
		mySprite = new Tga2D::CSprite("tga_logo.dds");
		mySprite->SetPosition(Tga2D::Vector2f(0.5f, 0.5f));
	}

	void CGameWorld::Update(float aTimeDelta)
	{
		mySprite->Render();
	}


Thats it! Compile and run and you should see something like this:

.. image:: /images/tutorial-2-1.png
