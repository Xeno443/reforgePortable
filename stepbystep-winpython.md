# reforgePortable
Experimenting to build a portable version of stable-diffusion-webui-reForge
This version uses the third-party WinPython portable version, which is recommended at various places and includes more stuff than the official
portable version. Maybe this provides more tools for installing additional extensions, and it has a negligibly larger footprint than the
official version. There is an even larger WinPython version, but I don't know what the differences are so we will go with the smaller one.

## Prerequisites
Microsoft Visual C++ 2015 Redistributable  
https://www.microsoft.com/en-us/download/details.aspx?id=48145  
Microsoft Visual C++ 2015-2022 Redistributable  
https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170#visual-studio-2015-2017-2019-and-2022  

***

## Prepare folders
1) Create folder C:\SD\reforge-portable
2) Create subfolder C:\SD\reforge-portable\system
3) Create subfolder C:\SD\reforge-portable\system\git
4) Create subfolder C:\SD\reforge-portable\system\python
![folder-2](https://github.com/user-attachments/assets/9a902582-fad3-4221-8246-d4874aeb4b66)

***
## Install Git portable
Browse to https://git-scm.com/downloads/win and download "64-bit Git for Windows Portable"  
![git-download-1](https://github.com/user-attachments/assets/1eaf8d60-2e0e-4775-9082-6b4934d42462)

Execute downloaded exe file and extract to C:\SD\reforge-portable\system\git  
![git-install-1](https://github.com/user-attachments/assets/03520868-5b3d-421f-9a37-d813719175bf)

***
## Install WinPython
Browse to https://github.com/winpython/winpython/releases/tag/6.1.20230527 and download "Winpython64-3.10.11.1dot.exe"
![winpython-download-1](https://github.com/user-attachments/assets/555f9b0d-1a6f-4f19-9494-d51881ea253e)

Run the downloaded executable and extract to a temporary directory. Select all files from "winpython\WPy64-310111\python-3.10.11.amd64"
![winpython-install-2](https://github.com/user-attachments/assets/79be1c7e-bf9c-4961-a0fa-347c5300e60d)

and copy them to "C:\SD\reforge-portable\system\python"
![winpython-install-3](https://github.com/user-attachments/assets/a00c87d6-71da-45e9-b7e3-11093a6fe633)

***
## Get run scripts
Open the forge standalone 7zip and extract only the 3 bat files from the root into C:\SD\reforge-portable  
![webui-install-1](https://github.com/user-attachments/assets/13d732b1-767a-41bd-acde-8b49c04e8a8d)

***
## Git clone reForge
Open cmd.exe in C:\SD\reforge-portable.
1) Run environment.bat
2) Run "git clone https://github.com/Panchovix/stable-diffusion-webui-reForge webui"
![webui-install-2](https://github.com/user-attachments/assets/cc1df314-fa1e-4323-b164-106be01e8220)

***
## First-run
Run "run.bat". This should now start the normal reForge requirements installations which may take quite a while  
![webui-install-3](https://github.com/user-attachments/assets/da8c3cb4-792c-46f7-82ee-5515eba77cf1)

If everything goes well the webUI page will open after everything is complete.





