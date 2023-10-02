# Handling Processes and Signals

This project focuses on understanding and working with process IDs (PIDs) and signals in Bash. It involves various tasks that utilize commands such as ps , pgrep , pkill , exit , and trap . Each task is described below:

## Task 0: What is my PID
- File: [0-what-is-my-pid](./0-what-is-my-pid)
- Description: This Bash script displays its own PID.

## Task 1: List your processes
- File: [1-list_your_processes](./1-list_your_processes)
- Description: This Bash script displays a list of currently running processes. It shows all processes for all users, including those without a TTY. The processes are displayed in a user-oriented hierarchy.

## Task 2: Show your Bash PID
- File: [2-show_your_bash_pid](./2-show_your_bash_pid)
- Description: This Bash script displays lines containing the keyword bash based on the script defined in 1-list_your_processes .

## Task 3: Show your Bash PID made easy
- File: [3-show_your_bash_pid_made_easy](./3-show_your_bash_pid_made_easy)
- Description: This Bash script displays the PID along with the process name of processes whose name contains the word bash .

## Task 4: To infinity and beyond
- File: [4-to_infinity_and_beyond](./4-to_infinity_and_beyond)
- Description: This Bash script displays the message To infinity and beyond indefinitely with a sleep 2 delay between each iteration.

## Task 5: Don't stop me now!
- File: [5-dont_stop_me_now](./5-dont_stop_me_now)
- Description: This Bash script kills the process created in [4-to_infinity_and_beyond](./4-to_infinity_and_beyond) using the kill command.

## Task 6: Stop me if you can
- File: [6-stop_me_if_you_can](./6-stop_me_if_you_can)
- Description: This Bash script kills the process created in [4-to_infinity_and_beyond](./4-to_infinity_and_beyond) using the pkill command.

## Task 7: Highlander
- File: [7-highlander](./7-highlander)
- Description: This Bash script displays the message To infinity and beyond indefinitely with a sleep 2 delay between each iteration. It also displays I am invincible!!! upon receiving a SIGTERM signal.

## Task 8: Beheaded process
- File: [8-beheaded_process](./8-beheaded_process)
- Description: This Bash script kills the process created in [7-highlander](./7-highlander).

## Task 9: Process and PID file
- File: [100-process_and_pid_file](./100-process_and_pid_file)
- Description: This Bash script creates the file /var/run/myscript.pid containing its PID and displays To infinity and beyond indefinitely. It also displays I hate the kill command upon receiving a SIGTERM signal and Y U no love me?! upon receiving a SIGINT signal. Finally, it deletes the file /var/run/myscript.pid and terminates itself upon receiving the SIGQUIT or SIGTERM signal.

## Task 10: Manage my process
- File: [manage_my_process](./manage_my_process)
- Description: This Bash script writes I am alive! to the file /tmp/my_process indefinitely with a two-second delay between each write. The script [101-manage_my_process](./101-manage_my_process) manages this script. When passed the argument start , it starts [manage_my_process](./manage_my_process), creates a file containing its PID in /var/run/my_process.pid , and displays manage_my_process started . When passed the argument stop , it stops [manage_my_process](./manage_my_process), deletes the file /var/run/my_process.pid , and displays manage_my_process stopped . When passed the argument restart , it stops [manage_my_process](./manage_my_process), deletes the file /var/run/my_process.pid , starts manage_my_process , creates a file containing its PID in /var/run/my_process.pid , and displays manage_my_process started . Otherwise, it displays Usage: manage_my_process {start|stop|restart} .

## Task 11: Zombie
- File: [102-zombie.c](./102-zombie.c)
- Description: This C program creates five zombie processes. For each zombie created, it displays Zombie process created, PID: <ZOMBIE_PID> .
