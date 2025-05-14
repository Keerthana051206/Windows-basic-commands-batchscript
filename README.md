# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\MyLab

![image](https://github.com/user-attachments/assets/240c07d5-9721-4a5c-8fb1-0f4ca4a188be)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![image](https://github.com/user-attachments/assets/a0bcb5c3-f909-4d70-be70-9a7532999203)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
type nul > MyFile.txt
![image](https://github.com/user-attachments/assets/b423c3f3-8f54-406c-aaa5-eb15487dd703)
List the contents of the "MyLab" directory
**COMMAND AND OUTPUT**
dir %userprofile%\Desktop\MyLab

![image](https://github.com/user-attachments/assets/2bb37417-ae68-4fd2-8f84-0663b55c194b)
Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
**COMMAND AND OUTPUT**
mkdir %userprofile%\Desktop\Backup
![image](https://github.com/user-attachments/assets/2024f63b-5783-4230-95e8-11d5f5b3ff21)

copy MyFile.txt %userprofile%\Desktop\Backup
![image](https://github.com/user-attachments/assets/66ddf4f4-5bb9-4396-8150-37fb16284068)


Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Documents

move MyLab Documents

![image](https://github.com/user-attachments/assets/ddcd6064-7400-4f90-b156-f7ab4c79626d)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.


**COMMAND**
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!

**OUTPUT**
![image](https://github.com/user-attachments/assets/454ff2dc-f0e8-4ba7-9008-de1923d8c0fe)


**COMMAND**
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully



## OUTPUT

![image](https://github.com/user-attachments/assets/5ffb1bf3-e535-475a-8ff0-4fde19b27a5a)




# RESULT:
The commands/batch files are executed successfully.

