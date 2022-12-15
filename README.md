# KDE - Dolphin - Remove Metadata  
## Protect your privacy
This adds a right click entry in Dolphin to remove all metadata / EXIF data from image files. This data can store information such as the photos GPS location and file servers it has been stored on.   
* Works with single and multiple images.  
* Easy to install
* Protects your privacy when sharing photos online.  
(You probably don't want to do this to all your photos as that data is useful for organizing them)
# Install
### Pre-Requisits
Requires [ExifTool](https://exiftool.org/) to be installed, for example:  
##### Ubuntu
* `sudo apt install libimage-exiftool-perl`  
##### Arch / Manjaro
* `sudo pacman -S perl-image-exiftool`  
##### Create a executable blank file
* `install -Dv /dev/null ~/.local/share/kio/servicemenus/removeMetadata.desktop`
##### copy the contents of removeMetadata.desktop from this repo into it
* `nano ~/.local/share/kio/servicemenus/removeMetadata.desktop`
* Save and quit Nano ( CTRL-O, CTRL-X )
##### Use it
* close any open dolphin sessions
* open dolphin
* right click a image or multiple images and select Remove Meta Data

## Screenshots
![Remove Metadata](screenshots/popup.png)  
### Before:
![Before](screenshots/before.png)  
### After:
![After](screenshots/after.png)
