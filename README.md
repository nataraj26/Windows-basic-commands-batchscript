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

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


mkdir %userprofile%\Desktop\MyLab

![image](https://github.com/ZafreenJagir/Windows-basic-commands-batchscript/assets/144870573/bae51f75-f6cf-48cf-b0e6-fbb3b6bdfa39)



## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.

cd %userprofile%\Desktop\MyLab

![image](https://github.com/ZafreenJagir/Windows-basic-commands-batchscript/assets/144870573/3fda6e27-edc8-4f39-a96c-5e49ee9103f5)


![image](https://github.com/ZafreenJagir/Windows-basic-commands-batchscript/assets/144870573/ee8aaf6a-bbaa-494f-b30c-1490967b620d)



## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.


dir %userprofile%\Desktop\MyLab

![image](https://github.com/ZafreenJagir/Windows-basic-commands-batchscript/assets/144870573/de4c5ce3-8d4b-4b95-bef5-667a1dd3f35e)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.


mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/ZafreenJagir/Windows-basic-commands-batchscript/assets/144870573/4386bf12-e3e7-49f5-a345-0456eefe6d83)


## COMMAND AND OUTPUT

mv Myfile.txt %userprofile%\Documents

![image](https://github.com/ZafreenJagir/Windows-basic-commands-batchscript/assets/144870573/256237bb-c5f7-40ec-a572-34a301827cff)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.


```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```


```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!

```



## OUTPUT

![image](https://github.com/ZafreenJagir/Windows-basic-commands-batchscript/assets/144870573/6e279804-b748-4593-a7b7-a9fbe3b6f227)




# RESULT:
The commands/batch files are executed successfully.

