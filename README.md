# reForge portable version experiment
[reForge](https://github.com/Panchovix/stable-diffusion-webui-reForge) being my favorite Stable Diffusion webUI but the last of the currently popular UIs without a portable version I wanted to see 
if I as a total python noob could build such a version, seeing as [Forge](https://github.com/lllyasviel/stable-diffusion-webui-forge) and [ComfyUI](https://github.com/comfyanonymous/ComfyUI) have
been available as such for quite some time.

**This version is not supported or endorsed by Panchovix!**

So I spent some time to figure out how the Forge portable version works, and after a bit of trial and error I recreated a reForge version from scratch. At first I tried to just plug reForge into the 
exisiting version but there were collisions as as both had different python module requirements the site-packages directory grew very large, so a fresh start was made.

During that I learned a lot of how this python pip thing works as it failed at various parts which later revealed that the original portable python zip version was somehow putting files in a different
directory than some things, most noticably the wheel build process, expected them to be.

### Download complete


### Download base


### Step by step for the official portable zip version
[stepbystep-pythonportable.md](stepbystep-pythonportable.md)

### Step by step for the WinPython version


