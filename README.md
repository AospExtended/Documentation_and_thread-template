# Documentation and Thread Template for AospExtended OS

![bannar7](https://raw.githubusercontent.com/AospExtended/Documentation_and_thread-template/10.x/Banner.png)

## Guidelines
Maintainers are asked to follow the guidelines mentioned below and for the thread template. Always take at least two reserved posts! Be respectful to users. If any fuss is created report us before doing anything.

[**Guidelines for Existing maintainer here**](https://github.com/AospExtended/Documentation_and_thread-template/blob/9.x/Maintainers_Rules.md).

## Adding Official Support

If you wish to maintain your device officially then read maintainer requirement mentioned below and make sure that you qualify before moving further or else you will be rejected.
If you fulfill the criteria mentioned below, fill out this [**maintainership form**](https://forms.gle/ChuuWeZnumc9H8He8) and wait for our response

## Maintainer Requirements
- MUST own the device(s).
- MUST be familiar with Github and have intermediate knowledge of it.
- MUST be able to Push/Pull and review changes on [Gerrit](http://gerrit.aospextended.com/).
- MUST be doing Unofficial build for at least 2-3 week before applying.
- MUST have their device(s) SELinux status as Enforcing.
- SHOULD have an XDA-thread for their current builds. If not, a link must be provided where they are providing support to users.
- SHOULD maintain proper authorship of commits in their device trees (device, kernel and vendor).

### Important Links:

<p align="center">
<img src="https://raw.githubusercontent.com/AospExtended/Documentation_and_thread-template/10.x/Banner.png" > 
</p>

AospExtended Twelve
===========
AospExtended is just an extension to AOSP, through which we 
are trying to provide a stock AOSP experience along with some important 
customization features. We have cherry-picked the features from many 
other projects and hence we are very thankful to them.

Credits
-------
* [**JDCTeam**](https://github.com/AOSP-JF-MM)
* [**DirtyUnicorns**](https://github.com/DirtyUnicorns)
* [**TeamSubstratum (Theme Engine)**](https://github.com/Substratum)
* [**LineageOS/Cyanogenmod**](https://github.com/LineageOS)
* [**Nitrogen Project**](https://github.com/nitrogen-project)
* [**ABC ROM**](https://github.com/ezio84)
* [**GZOSP**](https://github.com/GZOSP)
* [**Pure Nexus**](https://github.com/PureNexusProject)
* [**OmniROM**](https://github.com/omnirom/)
* [**AOSPA**](https://github.com/aospa/)
* [**BlissRoms**](https://github.com/BlissRoms)

How to Build?
-------------

To initialize your local repository using the AospExtended trees, use a 
command like this:

```bash
repo init -u git://github.com/AospExtended/manifest.git -b 12.x
```
To initialize a shallow clone, which will save even more space & time, use a command like this:

```bash
repo init --depth=1 -u git://github.com/AospExtended/manifest.git -b 12.x
```

Then to sync up:
----------------

```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
Finally to build:
-----------------

```bash
source build/envsetup.sh
lunch aosp_device_codename-userdebug
m aex -j$(nproc --all) | tee log.txt
```
## Report build issues
- For reporting bugs faced on officially supported devices, click [here](https://github.com/AospExtended/issue_tracker#issue-tracker-for-aospextended)

## Maintain Officially
- If you're building **AospExtended** for an unofficial device and would like to make it official, Check out the link below for more information about the requirements for both you and your device.
- [Click here for more info](https://github.com/AospExtended/Documentation_and_thread-template) (**Read full README**)

### Important Links:

- [Website](http://www.aospextended.com/)
- [Download Center](https://downloads.aospextended.com/)
- [Blog](https://blog.aospextended.com/)
- [Usage Statistics](https://stats.aospextended.com)
- [Gerrit Code Review](http://gerrit.aospextended.com/)
- [Documentation & Thread Template](https://github.com/AospExtended/Documentation_and_thread-template)
- [Bug Tracker](https://github.com/AospExtended/issue_tracker#issue-tracker-for-aospextended)
- [Extended Devices](https://github.com/AospExtended-devices/) 
- [Gallery](https://aospextended.com/gallery)
- [Telegram Channel](https://telegram.me/aospextended/)
- [Facebook page!](https://www.facebook.com/aospextended/)
- [Twitter](https://twitter.com/AospExtendedRom)
- [Help us translate AospExtended ROM and bring it to the world!](http://translate.aospextended.com/)
