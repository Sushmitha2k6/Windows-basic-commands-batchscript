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
```
mkdir %userprofile%\Desktop\MyLab
```

![1ma](https://github.com/user-attachments/assets/33d5a06e-cae9-4c77-8894-6734d89e594b)



Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```

![2ma](https://github.com/user-attachments/assets/87be7c05-71e2-499d-a938-f280a693772f)

type nul > MyFile.txt


![3ma](https://github.com/user-attachments/assets/ef764d3e-1358-4632-b15b-63c807a1dad1)


List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/55dd69af-fed6-41cd-8a49-549d5d026496)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/e3138f7a-05b6-4d70-9014-0c0a43653752)
```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/58b8f896-aa17-40e7-87e2-275213e444d0)


Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\Documents
```
![image](https://github.com/user-attachments/assets/cbc200c0-00e0-4959-bec7-0ae80420399d)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

![image](https://github.com/user-attachments/assets/d9e7d48a-b7ec-4017-8778-34317f77ae24)





## OUTPUT





# RESULT:
The commands/batch files are executed successfully.

