CS 4760 - Project 4: Project Scheduling
Rett Swyers

Intructions on how to run this file:
- use the "make" command to generate executable files for oss and worker
- worker will start a clock and terminate after a set amount of time, based on user input
- oss will immediately fork to create two processes, one will keep track of a global system time that the 
workers will use to keep track of, and the other will create as many worker processes that the user specifies
- to only run worker use the "./worker" and enter in the amount of seconds and nanoseconds you want it to run
for, such as "./worker 5 300000"
- to run oss, you can first run "./oss -h" to display this help message in the terminal. To specify how many 
workers to run, enter "-n" followed by a number. To specify how long each worker should run, enter "-s" 
followed by a number. To specify how long each worker will run for, enter "-t" followed by a number. To
specify the interval between each worker process, enter "-i" followed by a number. For example, you could 
enter "./oss -n 4 -s 2 -t 10 -i 3" to run 4 workers total, 2 at a time, for 10 seconds each, with each worker
starting every 3 seconds.
- After a total of 60 seconds, the program will close.