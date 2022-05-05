FalconOS 
===========
![FalconOS](https://github.com/Falcon-OS/Random_stuff/blob/main/falcon-banner.png)
<p align="center"> 

Fly Like Falcon ❤ 
===================

# Requirements
* 250GB Or More Disk Space 
* A computer with atleast 16GB Of Ram 
* 25GB+ Unsuable Internet 
* A Brain with Git Knowledge 
* Patience

# Preparing server
* Make Dir For Repo Binary: 
``` 
    mkdir ~/bin 
``` 

* Add directory for the repo binary to its path: 
```
    PATH=~/bin:$PATH 
``` 
* Downloading repo binary and placing it in the proper directory: 
``` 
   curl http://commondatastorage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
``` 
* Giving the repo binary the proper permissions 
``` 
   chmod a+x ~/bin/repo 
``` 
* Creating directory for where the ROM repo will be stored and synced 
```
    mkdir ~/falcon 
``` 
``` 
    cd ~/falcon 
```
 Getting Started 
--------------- 

To get started with Android, you'll need to get familiar with [Git and Repo](http://source.android.com/source/using-repo.html). To initialize your local repository using the Falcon trees, use a command like this: 
```
   repo init -u https://github.com/Falcon-OS/Android -b 12.L
``` 
To initialize a shallow clone, which will save even more space & time, use a command like this:
```
    repo init --depth=1 -u https://github.com/Falcon-OS/Android -b 12.L
```
Then to sync up: 
``` 
   repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
``` 
Building the source 
--------------- 
The source at Falcon is well configured for building. You can choose to build with or without gapps included. 
```
   . build/envsetup.sh 
``` 
Now Compile 
``` 
   lunch aosp_device_codename-userdebug 
``` 
Build 
``` 
   m falcon -j$(nproc --all)
``` 
Credits 
------- 
 * [**AOSP**](https://android.googlesource.com)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**PixelExperience**](https://github.com/PixelExperience)
 * [**ProtonAOSP**](https://github.com/ProtonAOSP)
 * [**ArrowOS**](https://github.com/ArrowOS)
 * [**ProjectElixir**](https://github.com/Project-Elixir)

# Telegram Support
[![Telegram](https://github.com/Lokesh773/RandomStuff/blob/master/Telegram_button.png)](https://telegram.me/joinchat/T5Bqs0DXTeLJeGpL)

