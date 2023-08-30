# ScriptClean

## Status: Alpha (testing)

## Description
ScriptClean is a Python utility designed to clean Python `.py` and PowerShell `.ps1` scripts. It removes unnecessary comments and blank lines to make your scripts more readable and efficient. The tool provides a user-friendly interface, complete with ASCII art, to guide you through the cleaning process. It leaves the,  comment and blank line, at the start of a function, but that will be the only, comments and blank lines, you will see :sunglasses:.

## Features
1. **ASCII Art Display**: Enhances the console output with visually appealing ASCII art.
2. **Directory Management**: Automatically creates the necessary directories ("Scripts", "Backup", "Cleaned") if they don't exist.
3. **File Scanning**: Scans the "./Scripts" folder for `.py` and `.ps1` files.
4. **User Interface**: Offers a numbered list of found script files for easy selection.
5. **File Backup**: Backs up the selected file to the "./Backup" folder before cleaning.
6. **File Cleaning**: Removes specific types of comments and blank lines based on user-defined rules.
7. **File Saving**: Saves the cleaned file to the "./Cleaned" folder.
8. **Original File Removal**: Deletes the original file from the "./Scripts" folder after cleaning.
9. **Statistics Display**: Shows statistics about the cleaning process, including the number of lines and comments removed.
10. **Looping Interface**: Allows continuous cleaning operations with options to clean another file or exit.

## Output
```
============================================================================
  _________            .__        __   _________ .__
 /   _____/ ___________|__|______/  |_ \_   ___ \|  |   ____ _____    ____
 \_____  \_/ ___\_  __ \  \____ \   __\/    \  \/|  | _/ __ \\__  \  /    \
 /        \  \___|  | \/  |  |_> >  |  \     \___|  |_\  ___/ / __ \|   |  \
/_______  /\___  >__|  |__|   __/|__|   \______  /____/\___  >____  /___|  /
        \/     \/         |__|                 \/          \/     \/     \/
============================================================================

 Scanning Folder...
 ...Scripts Found.

                       1. interface.py
                       2. model.py
                       3. utility.py
                       0. Clean All Sripts In Folder

 Select a file to clean (or 'quit' to exit):

```
```
 Cleaning Script...
 ...Script Cleaned.
                                    Stats:

Lines removed: 0
Comments removed: 2
Blank lines removed: 10
Total lines before: 150
Total lines after: 140
Percentage change in total lines: 6.67%

 Cleaning script...
 ...Script Cleaned.
                                    Stats:

Lines removed: 14
Comments removed: 7
Blank lines removed: 25
Total lines before: 158
Total lines after: 119
Percentage change in total lines: 24.68%

 Cleaning script...
 ...Script Cleaned.
                                    Stats:

Lines removed: 0
Comments removed: 0
Blank lines removed: 0
Total lines before: 105
Total lines after: 105
Percentage change in total lines: 0.00%

```
## Usage
1. Place the Python files you want to clean in the `./Scripts` folder.
2. Run `ScriptClean.bat` if you are on Windows for easy launching. Alternatively, you can run the Python script directly.
3. Follow the on-screen instructions to select a file for cleaning.
4. Review the cleaning statistics and either choose another file to clean or exit the program.

## Requirements
- Python 3.x
- Windows or Linux Operating System

## Notes
- The script automatically creates the necessary directories if they don't exist.
- Always back up important files before running any script that modifies them.

## Disclaimer
This tool is provided "as is" without any warranties. Always test the script on sample files before using it on important data. The authors are not responsible for any loss of data or functionality.
