
## Lab 04

- Name: Dan Gnau
- Email: gnau.11@wright.edu

## Part 1 - Task Tracker

Verify that `tt` made it to your GitHub repository for this course and is in your `Lab04` folder.  No answers will be written here unless you would like to leave a note to the TAs

## Part 2 - Sample Runs

### User Guide
```
Task Tracker (tt) User Guide
==============================
Available Functions
  tt add "<task_description>"  - Add a new task
  tt complete "<task_description>" - Complete a task
  tt view                       - View all tasks
  tt clear                      - Clear all tasks
  tt help                       - Show this help message

Examples:
  tt add "Walk the dog"
  tt complete "Walk the dog"
  tt view
  tt clear
```

### Sample runs

Example of using `add` task
```
./tt add "Walk the dog"

Task added: Walk the dogthe 
```

Example of using `complete` task
```
./tt complete "Walk the dog"

Task completed: Walk the dog
```

Example of using `view` tasks
```
./tt view

Tasks:
Walk the dog
Do the dishes
Mow the lawn
```

Example of using `clear` tasks
```
./tt add "Do the dishes"
./tt add "Mow the lawn"

./tt clear
Are you sure you want to remove all tasks? (y/n)
y
All tasks cleared.
```

Example of using `help`
```
./tt help

Task Tracker (tt) User Guide
==============================
Available Functions
  tt add "<task_description>"  - Add a new task
  tt complete "<task_description>" - Complete a task
  tt view                       - View all tasks
  tt clear                      - Clear all tasks
  tt help                       - Show this help message

Examples:
  tt add "Walk the dog"
  tt complete "Walk the dog"
  tt view
  tt clear
```

## Part 3 - PATH for all

- Chosen PATH directory: /usr/local/bin
- Link preference (hard or symbolic): symbolic
   - Justification of preference for this use case: it is much clearer that the file is linked when it is in symbolic form
- Command to create link: sudo ln -s ~pathtodirectory/tt /usr/local/bin/tt
- Notes about permissions modified: I used chmod 555 to ensure that anyone only has access to be able to read and execute the file
- How you tested that you can run `tt` from anywhere on filesystem: closed out of the initial terminal window it was created in, then ran it from a different directory
- How you tested that other users can run `tt`: I checked permissions to see -r-xr-xr-x, so everyone has access to read and execute. If I had another user set up on the computer I could log into that one and try it there.

## Extra Credit

Note here *what* you did to the script for the extra credit and provide additional demonstrations.

