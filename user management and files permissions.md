# User Management and File Permissions

## User Management

User management is one of the main tasks of Linux administrators. It involves creating, modifying, and deleting user accounts, as well as managing user permissions and access.

1. **Add User:**
   - This command is used to create a new user account.
   - syntax: `$ sudo adduser <username>`
    ![Add User](/assets/adduser.png)
   - Note: 
     - 'whoami' is used to display the current username.
     - 'su' command is used to switch user.

2. **Change User Password:**
   - To change user password in Linux, use the 'passwd' command.
   - syntax: `$ sudo passwd <username>`
   - ![Change User Password](/assets/usr_passwd_ch.png)

3. **Delete User:**
   - To delete a user in Linux, use the 'userdel' command.
   - syntax: `$ sudo userdel <username>`
   - ![Delete User](/assets/del_usr.png)

## Group Management

Group management involves creating, modifying, and deleting groups to organize users and define their collective permissions.

1. **Add Group:**
   - Syntax: `$ sudo addgroup <groupname>`
   - ![Add Group](/assets/add_group.png)

2. **Add User to Group:**
   - To add an existing user to a group: `$ sudo usermod -aG <groupname> <username>`
   - Note: '-aG' appends to the group list.
   - ![Add User to Group](/assets/adduser_to_grp.png)

3. **Delete Group:**
   - To delete a group: `$ sudo delgroup <groupname>`
   - Example of deleting a group:
    ![Delete Group](/assets/del_grp.png)

## File and Directory Permissions

Proper management of file and directory permissions is crucial for security and access control.

1. **Change Ownership:**
   - To change the ownership of a file or directory: `$ sudo chown <owner:group> <file or directory>`
   - ![Change Ownership](/assets/ch_ownership_grp.png)

2. **Change Permissions (Chmod):**
   - Files and directories have associated permissions represented by a series of letters and symbols.
   - ![Permissions Explanation](/assets/chmod.png)
   - **Symbolic Representation:** `$ sudo chmod u+rwx,g+rwx,o+rwx <filename>` ![Symbolic Permissions](/assets/symbolic.png)
   - **Numeric Representation:** `$ sudo chmod 777 <filename>` ![Numeric Permissions](/assets/numberic.png)

3. **Change Owner (Chown):**
   - To change the owner or group of a file or directory: `$ sudo chown <owner:group> <file_or_dir>`
   ![Change Owner](/assets/chown.png)

4. **Change Group (Chgrp):**
   - To change the group ownership of a file or directory: `$ sudo chgrp <groupname> <file_or_dir>`
   ![Change Group](/assets/chgrp.png)
