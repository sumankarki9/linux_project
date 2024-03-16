# User Management and File Permissions

## User Management

User management is one of the main tasks of Linux administrators. It involves creating, modifying, and deleting user accounts, as well as managing user permissions and access. Here are some basic commands related to user management:-

1. **Add User:**
    This command is used to create a new user account.
    syntax: `$ sudo adduser <username>`
    ![Add User](/assets/adduser.png)
    Note: 
     - 'whoami' is used to display the current username.
     - 'su' command is used to switch user.

2. **Change User Password:**
    To change user password in Linux, use the 'passwd' command.
    syntax: `$ sudo passwd <username>`
    ![Change User Password](/assets/usr_passwd_ch.png)

3. **Delete User:**
    To delete a user in Linux, use the 'userdel' command.
    syntax: `$ sudo userdel <username>`
    ![Delete User](/assets/del_usr.png)

## Group Management

Group management involves creating, modifying, and deleting groups to organize users and define their collective permissions.

1. **Add Group:**
    Syntax: `$ sudo addgroup <groupname>`
    ![Add Group](/assets/add_group.png)

2. **Add User to Group:**
    To add an existing user to a group: `$ sudo usermod -aG <groupname> <username>`
   - `NOTE`: '-aG' appends to the group list.
    ![Add User to Group](/assets/adduser_to_grp.png)

3. **Delete Group:**
    To delete a group: `$ sudo delgroup <groupname>`
   
    ![Delete Group](/assets/del_grp.png)
    

## File and Directory Permissions

Proper management of file and directory permissions is crucial for security and access control.

1. **Change Ownership:**
    To change the ownership of a file or directory: `$ sudo chown <owner:group> <file or directory>`
    ![Change Ownership](/assets/ch_ownership_grp.png)


   In this figure I have a directory named `test_dir` and a file named `testfile` . Initially, both were owned by the user `suman` and the group `suman`.

   After I use the `sudo chown` command to change the ownership of both `test_dir` and `testfile` to a new user named `testuser` and a new group named `testgroup` .

2. **Change Permissions (Chmod):**
   - Files and directories have associated permissions represented by a series of letters and symbols.
   - ![Permissions Explanation](/assets/chmod.png)
 
 
 a. In directories: 
    `drwxr-xr-x` :- this represent the type and permissions of the directory:-   

   `d` = directory
   `rwx`= permissions of the owner (testuser)
   `r-x`= permissions for the group (testgroup)
   `r-x` = permissions for others


 b. In files:
   `-rw-r–r– 1` :-this represent the type and permissions of the directory :- 


   -`-`  file
   -`rw` permissions of the owner (testuser)
   -`r`  permissions for the group       
   -`r`  opermissions for others


   -`NOTE`: First three permission like `rwx` for users. second three `rwx` for Group and other three `rwx` for others and it applies both file and directory.


Here’s the  detailed overview of symbolic and numeric representation in permission:-


   - **Symbolic Representation:**
   
    - `r` Read
    - `w` Write
    - `x` Execute
    - `-` No permission
   
   eg:  if we need to change the file permission to read, write and execute to all (user, group and others) in symbolic we use this command:-

   
    `$ sudo chmod u+rwx,g+rwx,o+rwx <filename>` !
    
    ![Symbolic Permissions](/assets/symbolic.png)

     


   - **Numeric Representation:**
   
    - `4` Read
    - `2` Write
    - `1` Execute
   eg:  if we need to change the file permission to read, write and execute to all (user, group and others) in numeric we use this command:-
   
    `$ sudo chmod 777 <filename>` ![Numeric Permissions](/assets/numberic.png)

3. **Change Owner (Chown):**
   - To change the owner or group of a file or directory: `$ sudo chown <owner:group> <file_or_dir>`
   ![Change Owner](/assets/chown.png)

4. **Change Group (Chgrp):**
   - To change the group ownership of a file or directory: `$ sudo chgrp <groupname> <file_or_dir>`
   ![Change Group](/assets/chgrp.png)