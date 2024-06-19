
# Practice Linux File Permissions

Welcome to the Practice Linux File Permissions repository! This is a show of my own practice of using read, write, and execute permissions in linux


## Basic File Permissions
- **Owner**: The user who owns the file.
- **Group**: Users who belong to the file's group.
- **Others**: Everyone else.

Each set of permissions consists of three characters:

- **r**: Read permission allows reading the contents of the file.
- **w**: Write permission allows modifying the file's contents.
- **x**: Execute permission allows executing the file (for executable programs or scripts) or accessing a directory.

## Viewing File Permissions

![image](https://github.com/YoriTano/Linux-file-permissions/assets/106491544/77bb4292-4e2b-4aca-811e-15662e1be250)


<b>The first line of the screenshot displays the command I entered, and the other lines display the output. The code lists all contents of the projects directory. I used the ls command with the -la option to display a detailed listing of the file contents that also returned hidden files. The output of my command indicates that there is one directory named drafts, one hidden file named .project_x.txt, and five other project files. The 10-character string in the first column represents the permissions set on each file or directory.</b>


![image](https://github.com/YoriTano/Linux-file-permissions/assets/106491544/07cde951-6947-4a7f-9287-00b7c92ba122)


<b>I know.project_x.txt is a hidden file because it starts with a period (.). In this example, I removed write permissions from the user and group, and added read permissions to the group. I removed write permissions from the user with u-w. Then, I removed write permissions from the group with g-w, and added read permissions to the group with g+r.</b>


![image](https://github.com/YoriTano/Linux-file-permissions/assets/106491544/b18a23fd-6c52-42f5-9c1f-5aa288f71f1d)


<b>I determined that the group had execute permissions, so I used the chmod command to remove them. The researcher2 user already had execute permissions, so they did not need to be added.</b>

<b>I changed multiple permissions to match the level of authorization my organization wanted for files and directories in the projects directory. The first step in this was using ls -la to check the permissions for the directory.I then used the chmod command multiple times to change the permissions on files and directories.</b>



