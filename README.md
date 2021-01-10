![TitaniumOS](https://github.com/Titanium-OS/manifest/raw/ten/TitaniumOS-banner.png)

# TitaniumOS #

Credits:
=======
 * [**AOSP**](https://android.googlesource.com)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**AOSiP**](https://github.com/AOSiP)
 * [**PixelExperience**](https://github.com/PixelExperience)

-----------------------------------------------------------------------------
Getting Started:
================

Create titanium folder:
----------------------

    mkdir ~/titanium
    cd ~/titanium
    

GIT config (nickname, e-mail):
-----------------------------

    git config --global user.email "mail@domain.com"
    git config --global user.name "login"
    

To initialize your local repository use:
---------------------------------------

    repo init -u git://github.com/TitaniumOS/manifest -b eleven
    

Then to sync up:
----------------

    repo sync -j$(nproc --all) --no-tags --no-clone-bundle

Build command is:
----------------
    . build/envsetup.sh
    lunch titanium_($device)-userdebug
    make titanium -j$(nproc --all)
    
Inheriting Gapps in build:
-------------------------
• To include Gapps in your builds, execute:
     export WITH_GMS=true
     
• For including stock gapps packages, execute:
     export TARGET_INCLUDE_STOCK_GAPPS=true
     
• For including pixel live wallpapers, execute:
     export TARGET_INCLUDE_LIVE_WALLPAPERS=true


## Report build issues
- You can reach us via [Telegram](https://t.me/TitaniumOS_Chat)

