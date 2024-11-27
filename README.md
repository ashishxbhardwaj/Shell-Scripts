# Shell-Scripts

## Update Script

pacman -Qtdq:Lists orphaned packages.
$(...): Passes the list of orphaned packages to pacman -Rns for removal.
-Rns: Removes the package and its unused dependencies.
--noconfirm: Skips confirmation prompts.
2>/dev/null: Silences error messages (if no orphaned packages).
|| echo "No orphaned packages to remove.": Displays a message if no orphaned packages are found.

