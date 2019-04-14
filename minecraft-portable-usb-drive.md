# How to make a portable Minecraft USB drive
## Requirments
1. a USB Drive
2. a Windows computer

## Before we begin
Before we begin, we need to format the usb drive with
NTFS. <br />
Plug in your USB Drive, and open file explorer. Now, right click on the USB drive and select "Format", and format the USB drive with NTFS.
## Downloading the launcher
First, we need to download the mineshafter launcher.
<br />
Go to https://mineshafter.info/downloads, download the launcher and copy it the USB drive.
create a folder called "data" in your USB drive.
now, press the windows key and R, type in "%appdata%" and press enter. copy the .minecraft folder into the data folder in your USB drive.
## Installing portable Java
go to https://portableapps.com/apps/utilities/java_portable, download the portable java installer, run it.and click "OK" and "next" until you see the following screen: <br />![alt text](https://i.imgur.com/gKjnjvz.png) <br />
Click on "browse" and choose your USB drive.
click on "install" and wait for it finish installing.
## Creating the start batch script
open notepad, type in the following:
```
@echo off
set APPDATA=data
start Java/bin/javaw.exe -jar Mineshafter-launcher.jar
```
and press CTRL + s, save it to the USB drive, make sure "Save as type" is set to "All files" and the filename is set to "start.bat".
## Running the game from the usb drive
Just plug it in and run start.bat
