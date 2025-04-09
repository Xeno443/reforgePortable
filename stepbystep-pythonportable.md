# reforgePortable
Experimenting to build a portable version of stable-diffusion-webui-reForge

Prerequisites:
Microsoft Visual C++ 2015 Redistributable  
https://www.microsoft.com/en-us/download/details.aspx?id=48145  
Microsoft Visual C++ 2015-2022 Redistributable  
https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170#visual-studio-2015-2017-2019-and-2022  

1) Create folder C:\SD\reforge-portable
2) Create subfolder C:\SD\reforge-portable\system
3) Create subfolder C:\SD\reforge-portable\system\git
4) Create subfolder C:\SD\reforge-portable\system\python
![folder-2](https://github.com/user-attachments/assets/9a902582-fad3-4221-8246-d4874aeb4b66)

***

Browse to https://git-scm.com/downloads/win and download "64-bit Git for Windows Portable"  
![git-download-1](https://github.com/user-attachments/assets/1eaf8d60-2e0e-4775-9082-6b4934d42462)

Execute downloaded exe file and extract to C:\SD\reforge-portable\system\git  
![git-install-1](https://github.com/user-attachments/assets/03520868-5b3d-421f-9a37-d813719175bf)

***

Browse to https://www.python.org/downloads/release/python-31011/ and download "Windows embeddable package (64-bit)"
![python-download-1](https://github.com/user-attachments/assets/732008ca-1d28-4320-8390-8e5ed4f7e028)

Extract downloaded zip file to C:\SD\reforge-portable\system\python  
![python-install-1](https://github.com/user-attachments/assets/50813c74-9c37-48fb-911a-269fe4940197)

Create subfolder C:\SD\reforge-portable\system\python\DLLs and move the following files from the python directory into this folder  
![python-install-2](https://github.com/user-attachments/assets/eb2a19ce-8ae0-4350-bca4-27f639f9cdb1)

Delete the file "python310._pth" from the C:\SD\reforge-portable\system\python directory  
![python-install-4](https://github.com/user-attachments/assets/9c224be6-cd0f-42a5-97d6-4c031ee6f023)


Browse to https://bootstrap.pypa.io/  (Github: https://github.com/pypa/get-pip) and download [get-pip.py](https://bootstrap.pypa.io/get-pip.py)  into C:\SD\reforge-portable\system\python 
![python-install-3](https://github.com/user-attachments/assets/0c9b4587-ad45-4310-a497-4034dfb2f762)

Open the forge standalone 7zip and extract only the 3 bat files from the root into C:\SD\reforge-portable  
![webui-install-1](https://github.com/user-attachments/assets/13d732b1-767a-41bd-acde-8b49c04e8a8d)

***

Open cmd.exe in C:\SD\reforge-portable.
1) Run environment.bat
2) Run "git clone https://github.com/Panchovix/stable-diffusion-webui-reForge webui"
![webui-install-2](https://github.com/user-attachments/assets/cc1df314-fa1e-4323-b164-106be01e8220)

Run "run.bat". This should now start the normal reForge requirements installations which may take quite a while  
![webui-install-3](https://github.com/user-attachments/assets/da8c3cb4-792c-46f7-82ee-5515eba77cf1)

If everything goes well the webUI page will open after everything is complete.





