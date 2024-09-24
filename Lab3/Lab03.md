
## Lab 03

- Name: Dan Gnau
- Email: gnau.11@wright.edu

## Part 1 Answers

1. `ssh` command before configuring `config` file: ssh -i ceg.pem ubuntu@3.221.20.238
2. HostName: 3.221.20.238
3. User: ubuntu
4. IdentityFile: ceg.pem
5. `~/.ssh/config` contents:

```
Host cegaws
    HostName 3.221.20.238
    User ubuntu
    Port 22

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
   - Explanation: prints DONE on a line by itself and outputs it to a file called "here.txt"
5. `ls -lt ~ | head`
   - Explanation: list the files in the home directory in long format, sort them by modification time, and uses the output to display the next 10 lines of input
6. `history | grep ".md"`
   - Explanation: show a list of previous commands used, uses it as the input, and grep will search for matching lines of code

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

1. PATH =
2. To set condition to `true`, I need to...
3. Command(s):
4. PATH =
   - Difference:
5. Command(s):
6. Commands & modification explanations: 
7. Script permission breakdown
   - User
      - must be:
      - has permissions to:
   - Group
      - must be:
      - has permissions to:
   - Other
      - has permissions to:

## Extra Credit

1. Note here *what* you did to the script for the extra credit.
