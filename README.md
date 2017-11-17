Have you ever had your smartphone full of trash files that you want to get rid of? Are cleaning apps unreliable to certain trash files?
If only there was a way to customize the files and folders that you want to delete... Oh wait, here's the solution!

These bash scripts allows users to delete their unwanted files (it can be anything) from their android device with one tap. Simply select the functions and the arguments that you want to use and run the script. Easy to use and effective when cleaning!

------

In order for this to work, you need:

1. Download and install [Terminal Emulator for Android](https://play.google.com/store/apps/details?id=jackpal.androidterm).
2. Put the folder with the scripts on a directory of your choice.
3. **ONLY MODIFY THE CLEAN_CACHE_USER FILE with the available functions.**
4. Put "_cd PATH_TO_LOCATION/clean_cache_android_" and "_sh CLEAN_CACHE_USER.sh_" as the initial command in the preferences to run the file everytime you open the Terminal.
5. Enjoy!
------

**Functions:**

* **_remove_type_**: delete files with the same extension from a certain folder
	* arguments:
		* 1st -> folder (full path)
		* 2nd to last -> extension type

* **_remove_**: delete files or folders
	* all arguments: file or folder (full path)

* **_remove_folder_**: remove certain folders within a directory
	* arguments:
		* 1st -> directory where the folders are (full path)
		* 2nd to last -> folders to delete (full path)

* **_remove_empty_files_folders_**: delete empty files and folders in the main folders and in all subfolders
	* arguments:
		* 1st -> main folder (full path)
		* 2nd to last -> folders and files to skip, if any (full path)

------

**WARNING: THESE BASH SCRIPTS CAN DELETE IMPORTANT FILES IF YOU DON'T KNOW HOW TO USE! I WILL NOT TAKE RESPONSIBILITY IF IMPORTANT DATA ON YOUR DEVICE IS LOST! USE IT AT YOUR OWN RISK!**

------

**Future implementations:**

| Priority | Description |
|----------------|:------------|
| Low | Adding counters for the number of files, folders and the total size of everything that was deleted (in a far future). |

------

**Versions:**

| Version number | Description |
|----------------|:------------|
| 2.3.2 | Fixed a bug on the last function, where at folders were not skipped. |
| 2.3.1 | Fixed bug in functions where not all arguments were parsed. |
| 2.3 | Altered the first 3 function in order to parse multiple arguments. |
| 2.2.1 | Fixed bug on "_remove_empty_files_folders_" function where it basically skipped the first argument as well. |
| 2.2 | Added the option to skip multiple files and folders in the function "_remove_empty_files_folders_". |
| 2.1 | Created a _README_ text file. |
| 2.0 | Separating functions and user preferences into two separate files. |
| 1.1 | Resolving problems with permissions. |
| 1.0 | Cleaning some junk code and making it "_look great_". |
| 0.6 | Added a condition in the "_remove_empty_files_folders_" function to skip certain folders. Its not fully implemented yet. |
| 0.5 | "_remove_empty_files_folders_" can now delete empty files and folders from subdirectories. |
| 0.4 | function "_remove_empty_files_folders_" created, but only working in the main folder, not the subfolders. |
| 0.3 | "_remove_type_" was added. |
| 0.2 | implemented function "_remove_folder_". |
| 0.1.1 | "_echo_" was added to the below function. |
| 0.1 | created "_remove_" function. |
