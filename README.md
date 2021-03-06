# Instagram Downloader

A python script to download public pictures, videos and albums from Instagram.

## Requirements
- Python (version 3.6 or higher)

## Features
- Download a single picture/video/album by running the script and providing the link as input
- Download a single picture/video/album by passing the link as a parameter to the script
- Download multiple pictures/videos/albums by passing a file list to the script (as parameter)
- No need to seperate pictures, videos and albums anymore, which was required in the old version
- Graphical User Interface: Do things the easy way!

## Usage

Examples:

- ### Download a single picture:
  ```shell
  ./instaload.py
  Please enter an URL to an instagram post e. g. https://www.instagram.com/p/BVKTcWWhyaS/
  https://www.instagram.com/p/BVKTcWWhyaS/
  ```
- ### Download a single picture using parameters:
  ```shell
  ./instaload.py https://www.instagram.com/p/BVKTcWWhyaS/
  ```
- ### Download multiple pictures using a filelist (e.g. links.txt):
  ```shell
  ./instaload.py links.txt
  ```
- ### Download videos/albums:
  Works the same way as downloading pictures! There's no need to specifiy if a post is a picture, video or album since the script can check that itself!
- ### Using the GUI:
  ```shell
  ./gui/instaload_gui.py
  ```
- ### Filter private links from public links for manual download:
  There is no need to do that anymore, script checks automatically now and creates a private link list if it encounters any!

  If you still want to use it (outdated):
  ```shell
  ./old/privateFilter.py links.txt
  ```
  Will create two files:
  - public.txt: contains all public links (pass this to one of the above scripts!)
  - private.txt: contains all private links (download these manually!)

## Changes to the old release:
- No OS dependency anymore: Runs on all platforms that support python3!
- Not dependent on shell anymore!
- No need to use different scripts and link lists for pictures/videos/albums!

Old release can still be found in [v0.9.0](https://github.com/michabirklbauer/instagram_downloader/tree/v0.9.0)!

## Credits
- Picture: [Unsplash - Lance Asper](https://unsplash.com/photos/3P3NHLZGCp8)
- Font: [Mightype Script](https://www.behance.net/gallery/29992721/Mightype-Script-Free-Handlettered-Font)
