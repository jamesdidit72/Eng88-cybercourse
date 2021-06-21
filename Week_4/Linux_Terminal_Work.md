# Linux 
## Commands

| Key(s) | Description | Example |
|:---------: |:----------------------------: |:--------: |
|Ctrl Alt T |for terminal in linux |  |
| mkdir | to create new directory |  |
| ls | lists everything in the current file path |  |
| type | prints what it is | type pwd = pwd in a shell builtin |
| man | help command | man ls |
| . | current directory | ./kali |
| touch | creates empty file | touch /folder/filename |
| echo  > | prints/ adds text to a file | echo text > filename |
| echo >> | appends to a file  | echo text >> filename |
| cat | prints contents | cat folder/filename |
| cp | copy a file | cp filename new filename |
| cp -r | copy directory | cp dirname new dirname -r |
| mv | move directory | mv dirname tootherdirname |
| rm -r | delete directory | rm -r dirname |
| cd | changes current directory | cd dirname |
| pwd | prints current directory |  |
| cd .. | goes to parent directory |  |
| history | prints history of inputs |  |
| date | prints date |  |
| df | shows file system |  |
| df -h | shows same stats in comprehendable format |  |
| top | shows live cpu usage |  |
| nano | to edit a file | nano filename |

### windows uses C: D: E: drives
### Linux uses root "/"
#### Linux works on the concept that everything is a file
#### one way of reading and writing
### extensions:
- used to make things clearer for the user
- linux doesnt care about extensions
    - cares about meta-data
### Control Permissions    
| Key(s) | Description | Example |
|:---------: |:----------------------------: |:--------: |
| ls -l | prints everything in the file path |  |
| sudo | allows for root commands to execute |  | 
| chmod | changes the permissions |  |
| chown | changes the ownership | chmod 000 filename | 
| cat/etc/passwd | prints all available users |  |

- r = read
- w = write
- x = execute
- "-" = no access
#### First character in line:
- d = directory
- "-" = file
    - permissions  
    - rwx   r-x   ---
    - user group other
