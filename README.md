# Shell-Scripts

## Update Script : 
A Bash script for updating an Arch Linux system. It prompts the user for confirmation, performs the system update, cleans up orphaned packages, and displays success or cancellation messages with ASCII art. Ideal for automating routine updates in a fun and interactive way.

`pacman -Qtdq` 
 >Lists orphaned packages.

`$(...)` 
 >Passes the list of orphaned packages to pacman -Rns for removal.

`-Rns` 
 >Removes the package and its unused dependencies.

`--noconfirm` 
 >Skips confirmation prompts.

`2>/dev/null` 
 >Silences error messages (if no orphaned packages).

`|| echo "No orphaned packages to remove."` 
 >Displays a message if no orphaned packages are found.

