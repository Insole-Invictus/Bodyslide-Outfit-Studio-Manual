**Uses:**
* OpenGL
* Simple OpenGL Image Library 2 - SOIL2
* TinyXML-2
* FSEngine (BSA/BA2 library)
* wxWidgets

**Compilation requirements:**
* Microsoft Visual C++ 2013
* wxWidgets 3.0.2+
* FBX SDK for VS2013: http://www.autodesk.com/products/fbx/overview

**Compiling with Visual Studio 2013:**

1. Download the wxWidgets source archive from https://www.wxwidgets.org/
2. Unpack it into a folder **"wxWidgets"** in your projects directory.
3. Open up **"..\wxWidgets\build\msw\wx_vc12.sln"** in Visual Studio 2013.
4. Set **/MTd** for the **Debug**, both **Win32** and **x64**, configurations of all projects in the solution.
5. Set **/MT** for the **Release**, both **Win32** and **x64**, configurations of all projects in the solution.
6. Build the **Debug** and **Release** configurations of the solution.
7. Get the **"GL/glext.h"** and **"GL/wglext.h"** header files from https://www.opengl.org/registry/
8. Copy them to **"%ProgramFiles(x86)%\Windows Kits\8.1\Include\um\gl"** (or without *(x86)* on 32-bit machine)
9. Open up the BodySlide solution in Visual Studio 2013 and build it.