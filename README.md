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
```
mkdir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/ddc7161b-2d83-4e0c-a391-bbec697eea53)



## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/8374423f-5938-4951-af68-f13429680d60)
![image](https://github.com/user-attachments/assets/97b9cca7-91a0-4922-b048-671bb8d2331a)



## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/0fe13e2a-f261-4e1d-9932-bdc65b70f614)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/f1b5f579-0801-4fb7-9752-f02264edb070)

![image](https://github.com/user-attachments/assets/637b0799-030d-4166-8bde-8ce1dc0d068e)


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/user-attachments/assets/b0166d48-a095-4227-99ad-c03d179b6861)



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

![image](https://github.com/user-attachments/assets/fafecf65-151a-4219-956d-712d7b07c092)




# RESULT:
The commands/batch files are executed successfully.

