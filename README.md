# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

NAME: ETTA SUPRAJA

REG NO: 212223220022

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

![image](https://github.com/user-attachments/assets/68c97c9b-d1aa-4326-b7c0-c64b5b86391f)

to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT

cd %userprofile%\Desktop\MyLab

![image](https://github.com/user-attachments/assets/e46cf3c5-95c4-4ad9-af79-7b57d5964ae9)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![image](https://github.com/user-attachments/assets/a46961a6-5ad7-4bdf-b7bb-3083872b8c6b)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/user-attachments/assets/a32cb113-a40b-4aae-809c-637c93cff1e0)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
mv Mylab %userprofile%\Documents

![image](https://github.com/user-attachments/assets/b5b12763-2151-40f2-a01e-c0186a2bb447)



## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```



## OUTPUT

![image](https://github.com/user-attachments/assets/7506f9eb-25b3-436d-9fa0-987db6c7055f)




# RESULT:
The commands/batch files are executed successfully.

