# Important commands on linux systems

## /etc/passwd

**This is a very important file on your system! It's used to keep track of all users on the system.**

Run cat /etc/passwd and look at the output; each line is organized in this format:

username:password:UID:GID:UID-info:home-directory:command/shell

Let’s run through what each of those mean:

1. username: the user’s login name
2. password: the password, will simply be an x if it’s encrypted
3. user ID (UID): the user’s ID number in the system. 0 is root, 1-99 are for predefined users, and 100-999 are for other system accounts
4. group ID (GID): Primary group ID, stored in /etc/group.
5. user ID info: Metadata about the user; phone, email, name, etc.
6. home directory: Where the user is sent upon login. Generally /home/
7. command/shell: The absolute path of a command or shell (usually /bin/bash). Does not have to be a shell though!
