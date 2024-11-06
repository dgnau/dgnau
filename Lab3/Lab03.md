
## Lab 03

- Name: Dan Gnau
- Email: gnau.11@wright.edu

## Part 1 Answers

1. `ssh` command before configuring `config` file: ssh -i /home/dgnau/ceg ubuntu@34.195.55.229
2. HostName: 3.221.20.238
3. User: ubuntu
4. IdentityFile: ceg.pem
5. `~/.ssh/config` contents:

```
Host cegaws
    HostName 3.221.20.238
    User ubuntu
    IdentityFile /home/dgnau/ceg
```

6. `ssh` command after configuring an entry in the `config` file: ssh cegaws

## Part 2 Answers

1. `printenv HOME > thishouse`
   - Explanation: will display the values of environtment values, in this case the value of HOME will be redirected to the "thishouse" file
2. `cat doesnotexist 2>> hush.txt`
   - Explanation: will attempt to read "doesnotexist", 2>> will redirect the standard error to a file named "hush.txt"
3. `cat nums.txt | sort -n >> all_nums.txt`
   - Explanation: reads "nums.txt", use it as an input, sort it numerically, and then output it to a file named "all_nums.txt"
4. `cat << "DONE" > here.txt`
   - Explanation: cat will read everything typed after the command, until DONE is typed by the user, into a document named "here.txt"
5. `ls -lt ~ | head`
   - Explanation: list the files in the home directory in long format, sort them by modification time, and uses the output to display the next 10 lines of input
6. `history | grep ".md"`
   - Explanation: show a list of previous commands used, uses it as the input, and grep will use the input to search for lines of code that contain the string ".md"

## Part 3

Verify that `roll` made it to your GitHub repository for this course and is in your `Lab03` folder.  No answers will be written here unless you would like to leave a note to the TAs

## Part 4 - Retrospective Answers

1. Where and when did it go wrong while working on your script tasks?
> I kept having divide by zero errors initally and my variable names did not match.
2. Was anything familiar working with a new language compared to one you are used to?
> Yes very much so. Java utilizes if loops in a similar way, printing errors to the user is similar (sorta), for loop formatting is very similiar.
3. Did you write good `commit` messages that refer to what tasks were completed at each commit?  What would you improve?
> No, I got ahead of myself and totally skipped over the part where I was supposed to commit after each change I made to the file. I only have the end result.

## Part 5 Answers

1. PATH = /usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin
2. To set condition to `true`, I need to... create a new bin directory
3. Command(s): `mkdir ~/bin`
4. PATH = /home/ubuntu/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin
   - Difference: the new value contains the new directory /home/ubuntu/bin
5. Command(s):
- `touch ~/bin/roll` **adds roll to bin**
- `cd ~bin` **changes the directory to bin**
- `chmod u+w ~/bin/roll` **changes the permissions of roll so I can write to it**
- `nano roll` **editor for roll**
6. Commands & modification explanations:
  `chmod +x ~/bin/roll` **I changed the permissions for roll to be executable anywhere**
7. Script permission breakdown
   - User
      - must be: the owner of the file
      - has permissions to: read, write, and execute the file
   - Group
      - must be: a member of the file's group
      - has permissions to: read, write, and execute the file
   - Other
      - has permissions to: read and execute the file (but cannot write to it)

## Extra Credit

1. I changed the text to appear red if an error occured.
