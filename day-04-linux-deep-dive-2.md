## Section 5: File Permissions

### Understanding Permissions
- d = directory
- - = regular file

- rwx = Owner permissions
- r-x = Group permissions
- r-- = Others permissions

- r = read = 4
- w = write = 2
- x = execute = 1

### Common Permission Numbers

- 777 = rwxrwxrwx = dangerous! never use
- 755 = rwxr-xr-x = scripts and folders
- 644 = rw-r--r-- = normal files
- 600 = rw------ = normal files
- 000 = -------- = no permissions

### Commands 

- chmod 644 file.txt = set permissions
- chmod +x script.sh = add exexute
- chmod -w file.txt = remove write
- chmod -R 755 folder = folder + contents
- chown user:group file = change owner

### Making Script Executable

- ./test.sh = permission denied 
- chmod +x test.sh = add permission
- ./test.sh = works now
