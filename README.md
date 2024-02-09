
# Linux Management

**Intially created a user called olatunji with its home directory as /home/olatunji `sudo useradd -s /bin/bash -m -d /home/olatunji olatunji`**

**Created 4 directory in the user home directory, Namely:**

- code
- tests
- personal
- misc

1. Change directory to the tests directory using absolute pathname: `cd /home/olatunji/tests`

1. Change directory to the tests directory using relative pathname:
   `cd ./tests`

1. Use echo command to create a file named fileA with text content 'Hello A' in the misc directory: `echo "Hello A" > fileA`

1. Create an empty file named fileB in the misc directory. Populate the file with a dummy content afterwards: `touch fileB; echo "This file is not empty`

1. Copy contents of fileA into fileC: `cp fileA fileC`

1. Move contents of fileB into fileD: `mv fileB fileD`
1. Create a tar archive callled misc.tar for the contents of misc directory: `tar -cvf misc.tar misc`
1. Compress the tar archive to create a misc.tar.gz file: `gzip misc.tar`
1. Create a user and force the user to change his/her password upon login: `sudo useradd -s /bin/bash -m -d /home/flash flash; sudo chage -d 0 flash`
1. Lock a users password: `sudo usermod -L flash`
1. Create a user with no login shell: `sudo useradd -s /sbin/nologin flashadmin`
1. Disable pasword based authentication for ssh: `PasswordAuthentication  no`
1. Disable root login for ssh: `PermitRootLogin no`
---
![linux screenshot](./images/Screenshot%202024-02-09%20155542.png)
---