# KDE - Dolphin - Remove Metadata

## Protect your privacy

This adds a right click entry in Dolphin to remove all metadata / EXIF data from image files. This data can store information such as the photos GPS location and file servers it has been stored on.   
* Works with single and multiple images.  
* Easy to install
* Protects your privacy when sharing photos online.  
(You probably don't want to do this to all your photos as that data is useful for organizing them)


## Install


### Prerequisites

Requires [ExifTool](https://exiftool.org/) and kdialog to be installed, for example:  

**Fedora**
- `sudo dnf install perl-Image-ExifTool kdialog`

**Ubuntu**
- `sudo apt install libimage-exiftool-perl kdialog`  

**Arch / Manjaro**
- `sudo pacman -S perl-image-exiftool kdialog`  

### Automatic Install

Install via Dolphin:

Dolphin -> Settings -> Configure Dolphin -> Context Menu -> Download New
Services -> Search for "Remove Metadata" -> Install "Remove Metadata" by merrittkr

### Manual Install

- Download the `removeMetadata.desktop` file
- Copy it to `~/.local/share/kio/servicemenus/`
- Restart Dolphin


## How to use

!!! There is no confirmation dialog, the metadata is removed immediately !!!

- Right click an image (or multiple images) and select `Remove Metadata` from the context menu


## Screenshots
![Remove Metadata](screenshots/popup.png)  

### Before:
![Before](screenshots/before.png)  

### After:
![After](screenshots/after.png)
