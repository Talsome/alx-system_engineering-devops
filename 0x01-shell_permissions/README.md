README

===
0 - Create a script that changes your user ID to betty. 
0-iam_betty
#!/bin/bash
su betty

===
1 - Write a script that prints the effective userid of the current user. 
1-who_am_i
#!/bin/bash
id -un

===
2 - Write a script that prints all the groups the current user is part of. 
2-groups
#!/bin/bash
groups

===
3 - Write a script that changes the owner of the file hello to the user betty. 
3-new_owner
#!/bin/bash
chown betty hello

===
4 - Write a script that creates an empty file called hello. 
4-empty
#!/bin/bash
touch hello

===
5 - Write a script that adds execute permission to the owner of the file hello. 
5-execute
#!/bin/bash
chmod u+x hello

===
6 - Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello. 
6-multiple_permissions
#!/bin/bash
chmod u+x,g+x,o+r hello

===
7 - Write a script that adds execution permission to the owner, the group owner and the other users, to the file hello 
7-everybody
#!/bin/bash
chmod ugo+x hello

===
8 - Write a script that sets the permission to the file hello as follows: 
8-James_Bond
#!/bin/bash
chmod 007 hello

===
9 - Write a script that sets the mode of the file hello to this: 
9-John_Doe
#!/bin/bash
chmod 753 hello

===
10 - Write a script that sets the mode of the file hello the same as olleh’s mode. 
10-mirror_permissions
#!/bin/bash
chmod --reference=olleh hello

===
11 - Create a script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed. 
11-directories_permissions
#!/bin/bash
chmod -R ugo+X .

===
12 - Create a script that creates a directory called dir_holberton with permissions 751 in the working directory. 
12-directory_permissions
#!/bin/bash
mkdir -m 751 my_dir

===
13 - Write a script that changes the group owner to holberton for the file hello 
13-change_group
#!/bin/bash
chgrp school hello

===
14 - Write a script that changes the owner to betty and the group owner to holberton for all the files and directories in the working directory. 
100-change_owner_and_group
#!/bin/bash
chown -hR vincent:staff .

===
15 - Write a script that changes the owner and the group owner of the file _hello to betty and holberton respectively. 
101-symbolic_link_permissions
#!/bin/bash
chown -h vincent:staff _hello

===
16 - Write a script that changes the owner of the file hello to betty only if it is owned by the user guillaume.
102-if_only
#!/bin/bash
chown --from=guillaume betty hello

===

