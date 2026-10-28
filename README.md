# Dell Latitude 7400 2-in-1 Hackintosh OpenCore

An OpenCore EFI repository for the Dell Latitude 7400 2-in-1.

> [!WARNING]
> I am not responsible for any damage done to your computer or for any lost data. Continue entirely at your own risk!

## Prerequisites

Before you begin, ensure you have the following:

- **Hardware:** Dell Latitude 7400 2-in-1 updated to the latest BIOS version.
- **Storage:** A 16 GB or larger USB drive.
- **Optional:** A secondary computer (highly recommended for creating the installer and troubleshooting).


## Creating the installer on macOS
macOS 13 and higher:
- Open terminal and paste this command: softwareupdate --list-full-installers; echo; echo "Please enter version number you wish to download:"; read REPLY; [ -n "$REPLY" ] && softwareupdate --fetch-full-installer --full-installer-version "$REPLY"
- Type in your designated macOS version number you wish to download
- Format your USB flash drive as macOS Extended and make the volume label MyVolume
- Paste this command in the terminal and edit it based on what version you downloaded: sudo /Applications/Install\ macOS\ Big\ Sur.app/Contents/Resources/createinstallmedia --volume /Volumes/MyVolume

macOS 12 and lower:
- Coming Soon!
## Creating the installer on Windows and Linux
- Search up com.apple.recovery.boot download and download your designated version
- Put the folder on the root with your USB

## Next, lets make the Opencore USB
- Download MountEFI and mount the EFI partition of your USB
- Grab an EFI from the release section of this repo based on the version of macOS you want to boot, then drag it to the mounted EFI partition
- Download OCAT and launch it
- Drag the config.plist file found in the USB/EFI/OC directory into the OCAT pane
- Go to Pl, and next to the Model Identifier dropdown menu, click Generate. This will generate a SMBIOS so your laptop doesn't conflict with other ones
- Save your config.plist


