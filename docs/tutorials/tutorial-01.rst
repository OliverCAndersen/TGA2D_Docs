Setup in visual studio
=======================

The engine consists of one solution containing three projects: **DX2DEngine**, **Game** and **Launcher**.


* DX2DEngine
	* This is the main project where everything engine related is.
* Game
	* This is where your game code will be.
* Launcher
	* This is a small project starting up your game code, which will then start the engine code

Start up the solution
^^^^^^^^^^^^^^^^^^^^^^
The project is always started via: ``TGA2D\Application\Application.sln`` (sln is important or your will se an empty project).

If you start it up it will load up all the projects.
Try rebuilding the solution in DEBUG.
It should compile (if not, see troubleshooting in the end of this document).
The engine is setup so it will create the exe files in: ``TGA2D\Bin``.
This is the place where all the data should be placed later (for example your ``Assets\`` folder).
The generated exe will be named either ``Launcher_Debug.exe`` or ``Launcher_Release.exe`` depending on your target build.
Two exes are always good so we don't mix them up when you send it to your artists.

.. warning:: Never send a debug exe to your artists!


Code tutorials
^^^^^^^^^^^^^^^^^^^^
We have some turorials set up as well.
Start them with ``Application_Tutorials.sln``.

