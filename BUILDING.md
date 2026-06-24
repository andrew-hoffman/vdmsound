Building this project requires a 32-bit Windows environment with Visual C++ 6.0 Enterprise Edition Service Pack 5, and the Windows 98 and XP DDKs. You will likely want to set up a Windows XP virtual machine for this purpose. 

Project files must be checked out from Git with CRLF line endings; set your `core.autocrlf` to true on Windows or the Visual Studioproject and workspace files (`.dsp` and `.dsw`) will not be openable. 

Build is done from inside Visual Studio, open the Workspace file inside VDMSCore or VDMSModules and select your build targets with Build -> Batch Build...

I will try to add proper overrides in a `.gitattributes` file to checkout only the text file types as CRLF on all OSes. Some binary files may have been improperly mangled by CVS/SVN.
