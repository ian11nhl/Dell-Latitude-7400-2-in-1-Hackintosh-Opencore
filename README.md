# Dell Latitude 7400 2-in-1 Hackintosh OpenCore

An OpenCore EFI repository for the Dell Latitude 7400 2-in-1.

> [!WARNING]
> I am not responsible for any damage done to your computer or for any lost data. Continue entirely at your own risk!

## Prerequisites

Before you begin, ensure you have the following:

- **Hardware:** Dell Latitude 7400 2-in-1 updated to the latest BIOS version.
- **Storage:** A 16 GB or larger USB drive.
- **Optional:** A secondary computer (highly recommended for creating the installer and troubleshooting).

**Creating the installer**
## On macOS
macOS 13 and higher:
- Open terminal and paste this command: softwareupdate --list-full-installers; echo; echo "Please enter version number you wish to download:"; read REPLY; [ -n "$REPLY" ] && softwareupdate --fetch-full-installer --full-installer-version "$REPLY"
- Type in your designated macOS version number you wish to download
macOS 12 and lower:
-
## On Windows

## On Linux



