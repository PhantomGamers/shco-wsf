# shco-wsf

 Widescreen fix for Sherlock Holmes Chapter One  

Removes in-game black bars and increases FOV to compensate.  
Does **NOT** remove black bars in cutscenes.  

## Screenshots

Before:
![SHCO_x17mB7l9un](https://user-images.githubusercontent.com/844685/142747093-f8f7ab0c-aa54-431c-83fe-2cb4c759266f.jpg)


After:
![SHCO_Aa6mdOHBgc](https://user-images.githubusercontent.com/844685/142747094-bb0041f0-fba2-4212-90d3-24246903cd5d.jpg)


## Install

To install, download the [latest release](https://github.com/PhantomGamers/shco-wsf/releases/latest) with your desired aspect ratio (SHCO-AR-VERSION.zip) and extract the contents of the zip so that the SH9 folder in the zip file gets merged with the SH9 folder in your Sherlock Holmes Chapter One installation folder.

## Configuration

This fix is based off of version 1.1.0 of my [Somewhat Universal Widescreen Fix](https://github.com/phantomgamers/suwsf).

You can edit the `SH9/Binaries/Win64/SUWSF.ini` file with your target resolution to change the AR that is set.

This is important for the 21:9 package because the various 21:9 aspect ratios (2560x1080, 3440x1440, and 3840x1600) are all slightly different. By default the 21:9 package comes configured for 3440x1440.

## Troubleshooting

If the Aspect Ratio change doesn't work (i.e. you still have black bars in-game), try renaming the `SH9/Binaries/Win64/dsound.dll` to another dll name marked as supporting `x64` on [this list](https://github.com/ThirteenAG/Ultimate-ASI-Loader#description)

If you get an error such as "Unable to load SUWSF.asi. Error:126", ensure you have the latest [64bit VC Redist installed](https://aka.ms/vs/17/release/vc_redist.x64.exe), alternatively use the [VisualCppRedist AIO](https://github.com/abbodi1406/vcredist) package which includes all versions of VC redist.

## Credits

- Thanks to [@RoseTheFlower](https://github.com/RoseTheFlower/) for helping me with the FOV calculations!
- [@DarthTon](https://github.com/DarthTon) for the Windows memory hacking library [Blackbone](https://github.com/DarthTon/Blackbone)
- [@ThirteenAG](https://github.com/ThirteenAG) for [IniReader](https://github.com/ThirteenAG/IniReader) and [UltimateASILoader](https://github.com/ThirteenAG/Ultimate-ASI-Loader)
