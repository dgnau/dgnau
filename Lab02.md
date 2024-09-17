## Lab 02

- Dan Gnau
- gnau.11@wright.edu

## Part 1 Answers

1. Command & steps to create an SSH key pair:
   1) open a terminal window
   2) use command ssh-keygen -t rsa
   3) When prompted, enter the location to save the file pairing to
   4) When prompted, enter a password to access the material (leave blank for no password)

2. Steps to add public key to GitHub profile:
   1) Login to GitHub
   2) Click on profile picture
   3) Click on settings
   4) Click on SSH and GPG keys
   5) Click the green "Add New SSH key" button
   6) Title Key & select key type
   7) Paste key identity into provided field
   8) Click the green "create key" button
3. git command to clone repository:
   git clone <https://github.com/dgnau/dgnau>

## Part 2 Answers

The answers for this section are to help you record what steps  
are needed to create a file locally (in your cloned repo)  
and push them (sync) with GitHub.  Only `git` commands are 
valid answers

1. git command to view the status of the repository: git status
2. git command example to add a file for tracking: git add <filename>
3. git command to commit changes: git commit -m "Commit message"
4. git command to sync local commits with GitHub: git push
5. git command to sync commits on GitHub to `clone`d repository: git pull

## Part 3 Answers

1. `chmod u+r bubbles.txt`
    - Means: changes the the file permissions for bubbles.txt to "user + read"
2. `chmod u=rw,g-w,o-x banana.cabana`
    - Means: changes the permissions for banana.cabana so that the user can read and write, the group can exclusively write, and so that others may only execute it
3. `chmod a=w snow.md`
    - Means: changes the permissions for snow.md so that all classes may write to it
4. `chmod 751 program`
    - Means: changes the permissions for a program so that the owner has all permissions, the group has read and excecute permissions, and others only have the execture permission
5. `chmod -R ug+w share`
    - Means: changes the permissions for all files recursively so that the user and group can write to it

## Part 4 Answers

1. Command to create new user: useradd "username"
2. Path to user's home directory: ~
3. Evaluate if `ubuntu` can add files to user's home directory: ls -l (then check to see if ubuntu has permissions)
4. Command to switch to user: su <username> followed by the password if requested
5. Command(s) to go to user's home directory: cd ~
6. Evaluate if user can add files to user's home directory: ls -l (check to see if user has permissions)
7. Command to switch to `ubuntu`: su ubuntu
8. Command to return to `ubuntu` home directory: ~ ubuntu

## Part 5 Answers

For each, write the command used or answer the question posed.

1. Command to create group named `crew`: sudo groupadd crew
2. Command(s) to add `ubuntu` & user to group `crew`: sudo useradd -g crew newuser
3. Command to modify `share` to have group ownership of `crew`: sudo chgroup share crew
4. Command to switch to user: su <username>
5. Command to add file to `share`: touch "filename" share
6. Evaluate why these steps allowed the above action: user was part of the group so they are allowed to add files 

## Part 6 Answers

For each, write the command used or answer the question posed.

1. Command to create file using `sudo`: sudo touch "filename" <filelocation>
2. Evaluate (in plain text) the permission of the file: -rw-r--r-- (user can read and write to the file while everyone else can read it)
3. Provide a method to edit the file without modifying permissions: sudo nano "filename" --- will pull up a text window to edit the file 
4. Command(s) to modify permissions: chmod (whatever permissions to assign to user/group/others)
