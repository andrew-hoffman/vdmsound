Building this project requires a 32-bit Windows environment with Visual C++ 6.0 Enterprise Edition Service Pack 5, and the Windows 98 and XP DDKs. You will likely want to set up a Windows XP virtual machine for this purpose. 

Project files must be checked out from Git with CRLF line endings or the Visual Studio project and workspace files (`.dsp` and `.dsw`) will not be openable. The `.gitattributes` file I have added to the project aims to enforce proper line endings on checkout for all relevant file types on all OSes. Some binary files may have been improperly mangled by CVS/SVN. On Windows you should set set your `core.autocrlf` global setting to true.

Building is done from inside Visual Studio, open the .dsw Workspace file inside VDMSCore or VDMSModules and select your build targets with Build -> Batch Build...
