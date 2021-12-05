# shco-wsf

 Widescreen fix for Sherlock Holmes Chapter One  

Removes in-engine black bars and switches FOV to hor+

[Rose also has a trainer that offers more control over the FOV](https://github.com/RoseTheFlower/SherlockHolmesCOUltrawide)

## Table of Contents

- [shco-wsf](#shco-wsf)
  * [Screenshots](#screenshots)
  * [Install](#install)
  * [Configuration](#configuration)
  * [Troubleshooting](#troubleshooting)
  * [Credits](#credits)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

## Screenshots

Before:
![SHCO_x17mB7l9un](https://user-images.githubusercontent.com/844685/142747093-f8f7ab0c-aa54-431c-83fe-2cb4c759266f.jpg)

After:
![SHCO_Aa6mdOHBgc](https://user-images.githubusercontent.com/844685/142747094-bb0041f0-fba2-4212-90d3-24246903cd5d.jpg)

## Install

1. **Ensure you have the latest [64-bit Microsoft Visual C++ Redistributable](https://aka.ms/vs/17/release/vc_redist.x64.exe) installed.**
2. Download the [latest release](https://github.com/PhantomGamers/shco-wsf/releases/latest/download/SHCO-WSF.zip)
3. Extract the contents of the zip so that the SH9 folder in the zip file gets merged with the SH9 folder in your Sherlock Holmes Chapter One installation folder.
4. *(Optional)* Edit `SH9/Binaries/Win64/SUWSF.ini` and set `Resolution=` to your monitor's resolution. This is only necessary if autodetection does not work for you.

## Configuration

This fix is based off of version 2.0 of my [Somewhat Universal Widescreen Fix](https://github.com/phantomgamers/suwsf).

You can edit the `SH9/Binaries/Win64/SUWSF.ini` file with your resolution if autodetection does not work for you.

## Troubleshooting

If you get an error such as "Unable to load SUWSF.asi. Error:126", ensure you have the latest [64bit VC Redist installed](https://aka.ms/vs/17/release/vc_redist.x64.exe).

If the Aspect Ratio change doesn't work (i.e. you still have black bars in-game), try renaming the `SH9/Binaries/Win64/dsound.dll` to another dll name marked as supporting `x64` on [this list](https://github.com/ThirteenAG/Ultimate-ASI-Loader#description)

## Credits

- Thanks to killer-m from WSGF discord for the dialogue pillarboxing and better FOV fix!
- Thanks to [@RoseTheFlower](https://github.com/RoseTheFlower/) for helping me with the FOV calculations for v1!
- [@ThirteenAG](https://github.com/ThirteenAG) for [Hooking.Patterns](https://github.com/ThirteenAG/Hooking.Patterns), [IniReader](https://github.com/ThirteenAG/IniReader) and [UltimateASILoader](https://github.com/ThirteenAG/Ultimate-ASI-Loader)
- [@sergey-shandar](https://github.com/sergey-shandar) for [getboost](https://github.com/sergey-shandar/getboost)
- [@codeplea](https://github.com/codeplea) for [tinyexpr](https://github.com/codeplea/tinyexpr)
