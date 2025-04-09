# reForge portable version experiment
[reForge](https://github.com/Panchovix/stable-diffusion-webui-reForge) being my favorite of Stable Diffusion webUI forks but not having portable version I wanted to see 
if I as a total python noob could build one, especially as [Forge](https://github.com/lllyasviel/stable-diffusion-webui-forge) and [ComfyUI](https://github.com/comfyanonymous/ComfyUI) have
had one available for quite some time.

**This version is not supported or endorsed by Panchovix! It's a personal experiment**

So I spent some time to figure out how the Forge portable version works, and after a bit of trial and error I recreated a reForge version from scratch. At first I tried to just plug reForge into the 
Forge version, but there were  some collisions as as both had different python module requirements and the site-packages directory grew very large, so I tried a fresh start.

During that I learned a lot of how this python pip thing works as it failed at some dependencies, which revealed that the original portable python zip version had a few files in a different
directory than some things, most noticably the wheel build process, expected them to be. Plus I was fighting some %path% issues that also lead to a file that needed to be deleted.

### Downloads
I have put three versions up for testing
- minimal: only has the portable git, python and the naked clone of the reForge repository and will download everything on first run
- torch: was run once and has all the python dependencies installed already
- custom: full install, plus updated UI settings for SDXL, a noobaiXL based checkpoint and some additional upscaler/adetailer modes already included
  I also pre-installed Forge Couple, Regional Prompter, ADetailer, tag autocomplete, LoraCTL and Dynamic Prompts

All three are made with reForge `f1.7.0-v1.10.1RC-latest-2177-g7dce877a`

As Github does not allow for files of this size so I put them on my Mega:
https://mega.nz/folder/w0p2WboI#zrAJMIxECeW0ER7v3X6eLg  
I will try to upload the minimal version to Github but I have to figure out how this LFS stuff works.

### Step by step for the official portable zip version
You should of course not simply trust a random stranger on the internet about anything, so if you don't want to use the prebuild packackes I also have documented step by step how I created these here:  
[stepbystep-pythonportable.md](stepbystep-pythonportable.md)
This version uses the official "Windows embeddable package (64-bit)" package. This seems to be a very minimal python version. I have no experience if this will be enough for each and every possible
extension of plugin that is available aout there.

### Step by step for the WinPython version


