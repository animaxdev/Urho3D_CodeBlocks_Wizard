# Urho3D_CodeBlocks_Wizard

An un-official template wizard for setting up Urho3D project on CodeBlocks.

Currently provides project setup for OpenGL, Direct3D9 and Direct3D11 using Mingw-w64 on Windows platform


#### Installation (Windows)
- Close Code::Blocks if its is open. Copy the folder named "urho3d" into Code::Blocks wizard folder. This wizard folder is located at `{Code::Blocks installation directory}/share/CodeBlocks/templates/wizard`

- Look for a file named "config.script" in the wizard folder and open it in a text editor. Locate the function RegisterWizards() and append the below line to it, probably at the end or any suitable place within it:
```
RegisterWizard(wizProject,_T("urho3d"),_T("Urho3D project"),_T("2D/3D Graphics"));
```
- Thats all. When you start Code::Blocks and select new projects you should see Urho3D template wizard there.

#### TODO
- Add support for MSVC++
- Add support for other platforms
