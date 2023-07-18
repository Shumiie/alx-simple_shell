 Everything you need to know to start coding your own shell

##TASKS
#[0. getppid (ppid.c)]
Write a program that prints the PID of the parent process. Run your program several times within the same shell. It should be the same. Doesecho $$ print the same value? Why? 
#[1. /proc/sys/kernel/pid_max (pid_max)
Write a shell script that prints the maximum value a process ID can be.
#[2. av (av.c)]
Write a program that prints all the arguments, without using ac.
#[3. Read line (read_line.c)]
Write a program that prints "$", wait for the user to enter a command, prints it on the next line.
#[4. command line to av (strtok.c)]
Write a function that splits a string and returns an array of each word of the string.
#[8. fork + wait + execve (fork.c), (wait.c), (exec.c)]
Write a program that executes the command ls -l /tmp in 5 different child processes. Each child should be created by the same process (the father). Wait for a child to exit before creating a new child
#[9.Super simple shell (shell.c)]
Using everything we saw, write a first version of a super simple shell that can run commands with their full path, without any argument.
#[10. find a file in the PATH]
Write a program that looks for files in the current PATH.
Usage: _which filename ...

#[11.0. printenv with environ (printenv.c)]
Write a program that prints the environment using the global variable environ.
#[11.1. env vs environ (environ.c)]
Write a program that prints the address of env (the third parameter of the main function) and environ (the global variable). Are they they same? Does this make sense?
#[11.2. getenv()]
Write a function that gets an environment variable. (without using getenv)
Prototype: char *_getenv(const char *name);
man 3 getenv
#[11.3. PATH]
Write a function that prints each directory contained in the the environment variable PATH, one directory per line.
#[11.4. PATH (path.c)]
Write a function that builds a linked list of the PATH directories.
#[11.5. setenv (setenv.c)]
Write a function that changes or adds an environment variable (without using setenv).
Prototype: int _setenv(const char *name, const char *value, int overwrite);
man 3 setenv
#[11.6. unsetenv (unsetenv.c)]
Write a function that deletes the variable name from the environment (without using unsetenv).
Prototype: int _unsetenv(const char *name);
man 3 unsetenv
