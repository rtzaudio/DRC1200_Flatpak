# DRC1200
DRC1200 linux Flatpak installer project files. 

This project is used to create the linux Flatpak installer for the DRC1200 software remote control application. The Flatpak builder pulls the wxWidgets libraries and the DRC1200 source code from the github repositories prior to building.

Execute the script './build_install.sh' to build and install the application on the development machine. If the build is good, then execute the script './build_bundle.sh' to create the standalone Flatpak install file 'DRC1200.flatpak'.

Users may download the flatpak file to their machine for installation. Then open a terminal and go to your user directory where the flatpak file resides and execute the following command to install:

'flatpak install DRC1200.flatpak'

By default, Flatpak installs applications system-wide (which may require sudo). If you want to install an application only for your current user account without root privileges, add the --user flag:

'flatpak --user install DRC1200.flatpak'

The DRC1200 application should be under the desktop menu "All Applications". right click to add the launcher to the desktop. You can also run it from the command line as follows:

'flatpak run org.flatpak.DRC1200'




