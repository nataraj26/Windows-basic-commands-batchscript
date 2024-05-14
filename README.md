# EX08 Windows-basic-commands-batchscript

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


## COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\MyLab
```
![mkdir](https://github.com/karthick-V-212223040086/Windows-basic-commands-batchscript/assets/149037461/e82e2f99-bead-4ce0-a456-acc495de960e)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT:
```
cd %userprofile%\Desktop\MyLab
```
![cd](https://github.com/karthick-V-212223040086/Windows-basic-commands-batchscript/assets/149037461/072bf08b-8f1f-47e7-9ce0-4bd5389e5e43)


```
type nul > MyFile.txt
```

![myfile](https://github.com/karthick-V-212223040086/Windows-basic-commands-batchscript/assets/149037461/72daf233-97b8-4bab-829b-4e43929a4fb1)




List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT:
```
dir %userprofile%\Desktop\MyLab
```
![dir](https://github.com/karthick-V-212223040086/Windows-basic-commands-batchscript/assets/149037461/ffa2b94b-cc47-478d-aaaf-e07201189f9f)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\Backup
```
![backup](https://github.com/karthick-V-212223040086/Windows-basic-commands-batchscript/assets/149037461/b398f90e-ae0b-4acd-9f4c-f61ecfe8cb82)

```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![copy](https://github.com/karthick-V-212223040086/Windows-basic-commands-batchscript/assets/149037461/98ab3063-d62a-4eb1-96a3-444a8d8aff5d)



Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\Documents

move MyLab Documents
```
![move](https://github.com/karthick-V-212223040086/Windows-basic-commands-batchscript/assets/149037461/342ac881-4ac9-4c2f-a6a0-cdc37248f16c)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.




## COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```


## OUTPUT:
![batch1](https://github.com/karthick-V-212223040086/Windows-basic-commands-batchscript/assets/149037461/c6377772-a55f-4d77-9d2c-78ea30ece3d9)


## COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT:
![modified batch1](https://github.com/karthick-V-212223040086/Windows-basic-commands-batchscript/assets/149037461/777c22b5-a3b1-444f-ad7a-045c05cd0d9c)

# RESULT:
The commands/batch files are executed successfully.

