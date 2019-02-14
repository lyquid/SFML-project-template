# SFML project template for Visual Studio and VS Code

Simple template config for quick starting and/or prototyping new [SFML](https://www.sfml-dev.org/index.php) projects in Microsoft's Visual Studio and Visual Studio Code.

## Configuring

You may want to change the following to suit your configuration.

In `SFMLtemplate.vcxproj` change the following lines to point to your SFML installation.

```
<AdditionalIncludeDirectories>C:\vs_dev_lib\SFML-2.5.1\include;%(AdditionalIncludeDirectories)</AdditionalIncludeDirectories>
//---
<AdditionalLibraryDirectories>C:\vs_dev_lib\SFML-2.5.1\lib;%(AdditionalLibraryDirectories)</AdditionalLibraryDirectories>
```

In `.vscode/c_cpp_properties.json` change the following lines to point to your SFML installation.
```
"includePath": [
  //---
  "C:\\vs_dev_lib\\SFML-2.5.1\\include"
],
```
Changing project and file's names can be a pain. For that, it's better to import the template file to Visual Studio and create a brand new project based on the template as suggested as follows.

## Adding the template to Microsoft Visual Studio

Copy the zip file `SFMLtemplate.zip` to `C:\Users\<YOURUSERNAME>\Documents\Visual Studio 2017\Templates\ProjectTemplates`.

Note that if you create a project this way, you must also manually copy `openal32.dll` to project root. 
This dll can be found in `\SFML-2.5.1\bin` from the original [SFML libraries](https://www.sfml-dev.org/download/sfml/2.5.1/).