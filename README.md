u# Top-100-Basic-Linux-Shell-Script-Examples
--------------------------------------------

@Day1. Hello, World!

   
#!/bin/bash
   
echo "Hello, World!"

📝 Prints a basic greeting message.

----------------------------------

@Day2:Display Current Date

#!/bin/bash

echo "Current date and time: $(date)"

📝 Uses the date command to show current system time.

-----------------------------------------------------

@Day3. Display Calendar

#!/bin/bash

cal

📝 Prints the current month's calendar.

----------------------------------------

@Day4. Print Current Working Directory

#!/bin/bash

pwd

📝 Displays the full path of the current directory.

----------------------------------------------------

@Day5. List Files in Current Directory

#!/bin/bash

ls -l

📝 Lists all files with details.

---------------------------------
@Day6. Take User Name and Greet

#!/bin/bash

read -p "Enter your name: " name

echo "Welcome, $name!"

📝 Prompts for a name and prints a welcome.

-------------------------------------------

@day7. Add Two Numbers

#!/bin/bash

read -p "Enter first number: " a

read -p "Enter second number: " b

sum=$((a + b))

echo "Sum is: $sum"

📝 Simple integer addition.

---------------------------


@day8. Check if File Exists

#!/bin/bash

read -p "Enter filename: " file

if [ -f "$file" ]; then

  echo "File exists."
  
else

  echo "File does not exist."
  
fi

📝 Checks for file presence.

----------------------------

@day9.

Check if Directory Exists

#!/bin/bash

read -p "Enter directory: " dir

if [ -d "$dir" ]; then

  echo "Directory exists."
  
else

  echo "Directory does not exist."
  
fi

📝 Validates if a folder exists.

---------------------------------

@day10. Create a File

#!/bin/bash

read -p "Enter filename to create: " file

touch "$file"

echo "File '$file' created."

📝 Creates an empty file.

------------------------------

@day11. Rename a File

#!/bin/bash

read -p "Old filename: " old

read -p "New filename: " new

mv "$old" "$new"

echo "File renamed."

📝 Renames a file.

---------------------------------

@day12. Delete a File

#!/bin/bash

read -p "Enter file to delete: " file

rm "$file"

echo "File deleted."

📝 Deletes a file.

-------------------------------------

@day13. Check Even or Odd Number

#!/bin/bash

read -p "Enter a number: " num

if (( num % 2 == 0 )); then

  echo "$num is even."
  
else

  echo "$num is odd."
  
fi

📝 Basic number check.

------------------------------------

@day14.  Use of For Loop

#!/bin/bash

for i in 1 2 3 4 5; do

  echo "Number: $i"
  
done

📝 Prints numbers using a loop.

----------------------------------

@day15. Use of While Loop

i=1

while [ $i -le 5 ]; do

  echo "Count: $i"
  
  ((i++))
  
done

📝 Repeats a block while a condition is true.

--------------------------------------------------

@day16. Basic Calculator

#!/bin/bash

read -p "Enter first number: " a

read -p "Enter operator (+ - * /): " op

read -p "Enter second number: " b

echo "Result: $((a $op b))"

📝 Simple arithmetic calculator.

---------------------------------

@day17. Read and Print File Content

#!/bin/bash

read -p "Enter file to read: " file

cat "$file"

📝 Displays the content of a file.

-------------------------------------

@day18. Count Words in a File

#!/bin/bash

read -p "Enter file name: " file

wc -w "$file"

📝 Prints number of words.

---------------------------

@day19.  Find Lines Matching Pattern

#!/bin/bash

read -p "Enter filename: " file

read -p "Enter pattern to search: " pattern

grep "$pattern" "$file"

📝 Finds matching lines using grep.

-------------------------------------

@day20.  Simple Menu System

#!/bin/bash

echo "1. Show Date"

echo "2. Show Uptime"

echo "3. Show Current Users"

read -p "Choose an option: " choice

case $choice in

  1) date ;;
     
  3) uptime ;;
     
  5) who ;;
     
  *) echo "Invalid option." ;;
  
esac

📝 Provides a simple text menu with case.

------------------------------------------

@day21.  Create a Directory

#!/bin/bash

read -p "Enter directory name: " dir

mkdir "$dir"

echo "Directory '$dir' created."

📝 Creates a new folder.

-------------------------

@day22.  Delete a Directory

#!/bin/bash

read -p "Enter directory name to delete: " dir

rmdir "$dir"

echo "Directory '$dir' deleted."

📝 Deletes an empty directory.

---------------------------------

@day23.  Loop Through Files in Directory

#!/bin/bash

for file in *; do

  echo "File: $file"
  
done

📝 Loops through and prints all files.

--------------------------------------

@day24. Check User Login

#!/bin/bash

read -p "Enter username: " user

if who | grep -w "$user" > /dev/null; then

  echo "User $user is logged in."
  
else

  echo "User $user is not logged in."
  
fi

📝 Checks if a user is currently logged in.

-------------------------------------------

day25. Show System Uptime

#!/bin/bash

uptime

📝 Displays how long the system has been running.

-------------------------------------------------

@day26. Check Root User

#!/bin/bash

if [ "$EUID" -eq 0 ]; then

  echo "You are root."
  
else

  echo "You are not root."
  
fi

📝 Checks if the script is being run as root.

---------------------------------------------

@day27. Countdown Timer

#!/bin/bash

for i in {5..1}; do

  echo "$i"
  
  sleep 1
  
done

echo "Time's up!"

📝 Simple countdown using a loop.

---------------------------------

@day28.  Convert Lowercase to Uppercase

#!/bin/bash

read -p "Enter text: " text

echo "${text^^}"

📝 Converts user input to uppercase.

------------------------------------

@day29. Convert Uppercase to Lowercase

#!/bin/bash

read -p "Enter text: " text

echo "${text,,}"

📝 Converts user input to lowercase.

------------------------------------

@day30.  Find File by Name

#!/bin/bash

read -p "Enter filename to search: " name

find . -name "$name"

📝 Searches for files recursively.

------------------------------------

@day31. Disk Usage of Directory

#!/bin/bash

read -p "Enter directory path: " dir

du -sh "$dir"

📝 Shows space used by a directory.

-----------------------------------

@day32. Get IP Address

#!/bin/bash

hostname -I

📝 Displays system's IP address.

--------------------------------

@day33. Show Currently Running Processes

#!/bin/bash

ps aux

📝 Displays all running processes.

--------------------------------------

@day34. Kill a Process by Name

#!/bin/bash

read -p "Enter process name to kill: " pname

pkill "$pname"

📝 Terminates all processes matching the name.

----------------------------------------------

@day35. Backup a File

#!/bin/bash

read -p "Enter filename to backup: " file

cp "$file" "$file.bak"

echo "Backup created as $file.bak"

📝 Creates a .bak copy of a file.

---------------------------------------

@day36. Simple Login Prompt

#!/bin/bash

read -p "Username: " user

read -sp "Password: " pass

echo -e "\nWelcome, $user!"

📝 Simulates a login prompt (no password checking).

----------------------------------------------------

@day37. Display Memory Usage

#!/bin/bash

free -h

📝 Shows system memory usage in human-readable format.

------------------------------------------------------

@day38.  Display Disk Usage

#!/bin/bash

df -h

📝 Displays disk usage of all mounted partitions.

--------------------------------------------------

@day39. Append Text to a File

#!/bin/bash

read -p "Enter file to append to: " file

read -p "Enter text: " text

echo "$text" >> "$file"

echo "Text appended to $file."

📝 Appends user input to a file.

-----------------------------------

@day40. Check If File Is Empty

#!/bin/bash

read -p "Enter file name: " file

if [ ! -s "$file" ]; then

echo "File is empty."

else

echo "File is not empty."

fi

📝 Checks if a file has content or not.

----------------------------------------

@day41. Reverse a String

#!/bin/bash

read -p "Enter a string: " str

echo "$str" | rev

📝 Reverses the characters in the string.

------------------------------------------

@day42. Check String is Palindrome

#!/bin/bash

read -p "Enter a string: " str

rev_str=$(echo "$str" | rev)

if [ "$str" == "$rev_str" ]; then

echo "Palindrome"

else

echo "Not a palindrome"

fi

📝 Compares original and reversed strings.

-------------------------------------------

@day43. Count Number of Lines in a File

#!/bin/bash

read -p "Enter filename: " file

wc -l < "$file"

📝 Counts total lines in the file.

----------------------------------

@day44. Check Whether Input is a Number

#!/bin/bash

read -p "Enter something: " input

if [[ "$input" =~ ^[0-9]+$ ]]; then

  echo "It's a number."
  
else

  echo "Not a number."
  
fi

📝 Uses regex to check numeric input.

--------------------------------------

@day45.Print All Environment Variables

#!/bin/bash

printenv

📝 Shows current environment variables.

---------------------------------------

@day46. Set and Use a Variable

#!/bin/bash

greeting="Hello from Linux!"

echo "$greeting"

📝 Demonstrates defining and using a shell variable.

----------------------------------------------------

@day47.  Use of Arrays

#!/bin/bash

fruits=("apple" "banana" "cherry")

echo "First fruit: ${fruits[0]}"

echo "All fruits: ${fruits[@]}"

📝 Works with array elements.

---------------------------------

@day48. Loop Over Array

#!/bin/bash

colors=("red" "green" "blue")

for color in "${colors[@]}"; do

echo "Color: $color"

done

📝 Prints all elements of an array.

-------------------------------------

@day49.  Check File Permissions

#!/bin/bash

read -p "Enter filename: " file

ls -l "$file"

📝 Lists file with its permission details.

---------------------------------------------

@day50. Check Internet Connection

#!/bin/bash

ping -c 1 google.com &> /dev/null

if [ $? -eq 0 ]; then

echo "Internet is connected."

else

  echo "No internet connection."
  
fi

📝 Pings Google to check connectivity.

---------------------------------------

@day51. Check if Package is Installed (Debian-based)

#!/bin/bash

read -p "Enter package name: " pkg

dpkg -l | grep "$pkg"

📝 Lists installed packages and filters by name.

-----------------------------------------------------

@day52. Display Number of Users Logged In

#!/bin/bash

who | wc -l

📝 Counts active user sessions.

--------------------------------------

@day53. Send Message to Another Logged-in User

#!/bin/bash

read -p "Enter username: " user

read -p "Enter your message: " msg

echo "$msg" | write "$user"

📝 Sends message to another terminal user (if write is enabled).

--------------------------------------------------------------------

@day54. Change File Permissions

#!/bin/bash

read -p "Enter filename: " file

chmod 755 "$file"

echo "Permissions changed to 755."

📝 Makes a script executable by all users.

------------------------------------------------

@day55. Create a Simple Log File

#!/bin/bash

echo "Log Entry at: $(date)" >> script.log

📝 Appends a timestamped line to a log file.

---------------------------------------------

@day56. Clear the Terminal Screen

#!/bin/bash

clear

📝 Clears the terminal window.

--------------------------------

@day57. Compare Two Numbers

#!/bin/bash

read -p "Enter first number: " a

read -p "Enter second number: " b

if [ "$a" -gt "$b" ]; then

  echo "$a is greater"
  
elif [ "$a" -lt "$b" ]; then

  echo "$b is greater"
  
else

  echo "Both are equal"
  
fi

📝 Performs a numeric comparison.

----------------------------------

@day58.  Find Factorial of a Number

#!/bin/bash

read -p "Enter a number: " n

fact=1

for (( i=1; i<=n; i++ )); do

  fact=$((fact * i))
  
done

echo "Factorial is $fact"

📝 Computes factorial using a loop.

------------------------------------

@day59. Generate Random Number

#!/bin/bash

echo "Random number: $RANDOM"

📝 Generates a random number using shell built-in.

--------------------------------------------------

@day60.  Check Disk Space Usage of Root Partition

#!/bin/bash

read -p "Enter a number: " n

sum=0

for (( i=1; i<=n; i++ )); do

  sum=$((sum + i))
  
done

echo "Sum = $sum"

📝 Adds numbers from 1 to n.

----------------------------

@day61.  Sum of N Natural Numbers

#!/bin/bash

read -p "Enter a number: " n

sum=0

for (( i=1; i<=n; i++ )); do

  sum=$((sum + i))
  
done

echo "Sum = $sum"

📝 Adds numbers from 1 to n.

-----------------------------

@day62.Print Multiplication Table

#!/bin/bash

read -p "Enter a number: " n

for i in {1..10}; do

echo "$n x $i = $((n * i))"

done

📝 Prints a 10-row multiplication table.

----------------------------------------------

@day63.Check Leap Year

#!/bin/bash

read -p "Enter year: " year

if (( (year % 4 == 0 && year % 100 != 0) || year % 400 == 0 )); then

echo "$year is a leap year."

else

echo "$year is not a leap year."

fi


📝 Validates leap year logic.

------------------------------------------------------------------

@day64.  Find Largest of Three Numbers

#!/bin/bash

read -p "Enter 3 numbers: " a b c

if [ $a -ge $b ] && [ $a -ge $c ]; then

  echo "$a is largest"
  
elif [ $b -ge $a ] && [ $b -ge $c ]; then

  echo "$b is largest"
  
else

  echo "$c is largest"
  
fi

📝 Compares three values.

---------------------------------------

@day65.Simple Number Guessing Game

#!/bin/bash
secret=$((RANDOM % 10 + 1))
read -p "Guess a number (1-10): " guess
if [ "$guess" -eq "$secret" ]; then
  echo "Correct!"
else
  echo "Wrong. The number was $secret"
fi

📝 Fun use of random and conditional logic.

-------------------------------------------

@day66.  Check If Port Is Open

#!/bin/bash
read -p "Enter hostname: " host
read -p "Enter port: " port
nc -zv "$host" "$port"

📝 Checks if a port is open using netcat.


-------------------------------------------

@day67.Run Script at Startup (Cron @reboot Example)

#!/bin/bash

(crontab -l ; echo "@reboot /path/to/your/script.sh") | crontab -


📝 Schedules a script to run when system starts.

----------------------------------------------------------------

@day68. Shutdown System After Delay

#!/bin/bash

read -p "Shutdown after how many minutes? " min

sudo shutdown -h +$min

📝 Schedules a shutdown using shutdown command.

-------------------------------------------------

@day69. Create Multiple Files

#!/bin/bash

for i in {1..5}; do

  touch "file$i.txt"
  
done

📝 Creates 5 empty files.

-------------------------

@day70. Monitor File Changes

#!/bin/bash

read -p "Enter filename: " file

inotifywait -m "$file"

📝 Watches file changes in real-time (requires inotify-tools).

--------------------------------------------------------------

@day71. Simple Progress Bar

#!/bin/bash

echo -n "Progress: "

for i in {1..20}; do

  echo -n "#"
  
  sleep 0.1
  
done

echo " Done!"

📝 Shows a loading bar animation.

----------------------------------



@day72. Backup a Directory

#!/bin/bash

read -p "Enter directory to backup: " dir

tar -czf backup.tar.gz "$dir"

echo "Backup saved as backup.tar.gz"

📝 Creates a compressed backup file.

------------------------------------

@day73. Count Specific Word in File


#!/bin/bash
read -p "Enter filename: " file
read -p "Enter word to count: " word
grep -o "$word" "$file" | wc -l

📝 Counts how often a word appears.

------------------------------------

@day74. Rename All .txt Files to .bak

#!/bin/bash

for file in *.txt; do

  mv "$file" "${file%.txt}.bak"
  
done

📝 Batch renaming using parameter expansion.

---------------------------------------------

@day75. Find Files Modified Today

#!/bin/bash

find . -type f -mtime -1

📝 Lists files modified in the last 24 hours.

---------------------------------------------

@day76.  Count Characters in a String

#!/bin/bash

read -p "Enter a string: " str

echo "Length: ${#str}"

📝 Uses parameter expansion to get string length.

--------------------------------------------------

@day77. Run a Command Every 5 Seconds


#!/bin/bash

while true; do

date

sleep 5

done

📝 Loop with delay – useful for monitoring.

-------------------------------------------

@day78.  Monitor CPU Usage

#!/bin/bash

top -bn1 | grep "Cpu(s)"

📝 Extracts CPU usage info using top.

-------------------------------------

@day79. Monitor Memory Usage (Real-Time)

#!/bin/bash

watch free -m

📝 Refreshes memory info every 2 seconds.

-----------------------------------------

@day80.Simple Alarm Clock

#!/bin/bash

read -p "Set alarm (seconds): " sec

sleep "$sec"

echo -e "\aTime's up!"

📝 Plays a beep sound after delay

-----------------------------------
@day81. Check Service Status

#!/bin/bash

read -p "Enter service name: " svc

systemctl status "$svc"

📝 Shows status of a systemd-managed service.

-----------------------------------

@day82. Start a Service

#!/bin/bash

read -p "Enter service name: " svc

sudo systemctl start "$svc"

echo "$svc started."

📝 Starts a system service (requires sudo).

-------------------------------------------

@day83. Stop a Service

#!/bin/bash

read -p "Enter service name: " svc

sudo systemctl stop "$svc"

echo "$svc stopped."

📝 Stops a running service.

-------------------------------------------
@day84. Restart a Service

#!/bin/bash

read -p "Enter service name: " svc

sudo systemctl restart "$svc"

echo "$svc restarted."

📝 Restarts a service quickly.

-------------------------------

@day85.Get Current Date and Time

#!/bin/bash

date "+%Y-%m-%d %H:%M:%S"

📝 Formats the current date and time.

-------------------------------------

@day86. Display Calendar

#!/bin/bash

cal


📝 Shows the current month calendar.

------------------------------------
@day87. Extract .tar.gz File


-------------------------------------
