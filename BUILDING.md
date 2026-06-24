Building this project requires a 32-bit Windows environment with Visual C++ 6.0 Enterprise Edition Service Pack 5, and the Windows 98 and 2k DDKs. You will likely want to set up a Windows 2000 or XP virtual machine for this purpose. 

Project files must be checked out from Git with CRLF line endings or the Visual Studio project and workspace files (`.dsp` and `.dsw`) will not be openable. The `.gitattributes` file I have added to the project aims to enforce proper line endings on checkout for all relevant file types on all OSes. Some binary files may have been improperly mangled by CVS/SVN. On Windows you should set set your `core.autocrlf` global setting to true.

Add a VDMSCorePath environment variable pointing to the VDMSCore directory inside the source tree.

Building is done from inside Visual Studio, open the .dsw Workspace file inside VDMSCore or VDMSModules and select your build targets with Build -> Batch Build...

Borland C++ 5.5 16-bit compiler is needed to build the Win9x DOSDRV.EXE, and the BCPATH environment variable must point to this install location. 

"Just make dummy dosdrv.obj and dosdrv.exe and touch them to be newer than the source and MSVC will skip that part of the build.
You will need pieces of the NT4/2k DDK (vintage by now) and set up some env vars in MSVC to point to them (see the include and lib of the project.) that's prolly where the idl etc. errors come from."  -vladr
