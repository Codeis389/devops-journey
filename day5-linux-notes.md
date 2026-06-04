## Section 7: User Management

- whoami = show current user
- who / w = logged in users
- cat /etc/passwd = all user list
- sudo useradd -m -s /bin/bash name = create user
- sudo passwd name = set password
- su - name = switch to user
- sudo usermod -aG sudo name = create to user
- sudo groupadd name = create group
- groups name = show user's groups
- sudo userdel -r name = delete user + home folder

## Rule: Never run apps as root, least privilage


## Section 8: Service Management
- systemctl status name = check service status
- systemctl start name = start service
- systemctl stop name = stop service
- systemctl restart name = restart service
- systemctl enable name = auto start on boot
- systemctl disable name = don't auto start
- systemctl --failed = show crashed services
- journalctl -u name -n 50 = last 50 lines of logs
- journalctl -u name -f = live service logs

## Rule: After installing any service:
## enable = start = status


# Bash Scripting

## Section 1: First Script

- #!/bin/bash = shebang, always first line
- echo "text" = print text
- chmod +x script.sh = make execcutable
- ./script.sh = run script

## Section 2: Variables
- Name="value" = create variable
- echo $Name = use variable
- $USER = current user
- $HOME = home directory
- $PWD = current directory

## Section 3: User INput
-read NAME = wait for input
- read -p "message" NAME = show message then input

## Section 4: If/Else Conditions
- if [ $VAR -ge 90 ] = if greater or equal
- elif [ condition ] = else if
- else = otherwise
- fi = end of if

## Comparison Operators
- -eq = equal
- -ne = not equal
- -gt = greater than
- lt = less than
- -ge = greater or equal
- -le = less or equal

## Rule: Always spces insdie [] brackets!
## if [ condition ] = this is wrong approach
## if[condition ] = this is right approach


# Day 4 - Bash Scripting

## Section 1: First Script

- #!/bin/bash = create variable
- echo "text" = print text
- chmod +x script.sh = make executable
- ./script.sh = run script

## Section 2: Variables
- Name="value" = create variable
- echo $NAME = use variable
- $USER = current user
- $HOME = home directory
- $PWD = current directory

## Section 3: User Input
- read NAME = wait for input
- read -p "msg" NAME = show message then input

## Section 4: If/Else Conditions
- if [ $VAR -ge 90 ] = if greater or equal
- elif [ condition ] = else if
- else = otherwise
- fi = end of if
- Rule: Always spaces inside [] brackets!

## Comparison Operators

- -eq = equal
- -ne = not equal
- -gt = greater than
- -lt = less than
- -ge = greater or equal
- -le = less or equal

## Section 5: Loops

- For i in {1..10} = loop 1 to 10
- for i in $LIST = loop through list
- while [ condition ] = while loop
- do / done = loop body

## Section 6: Functions

- function_name() {} = define function
- function_name = call function
- $1, $2 = function parameters

## Section 7: Real DevOps Scripts
- back.sh = auto backup files
- healthcheck.sh = monitor server health
- clearnup.sh = auto clean server
- devops-automation.sh = menu driven automation

## What I learned in Day 4:
- Write automation scripts
- Combine variables + conditions + loops + functions
- Build real DevOps tools from scratch
