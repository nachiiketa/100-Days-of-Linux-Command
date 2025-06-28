# Top-100-Basic-Linux-Shell-Script-Examples
-------------------------------------------

@Day1. Hello, World!
   
#!/bin/bash
   
echo "Hello, World!"

📝 Prints a basic greeting message.

-----------------------------

@Day2:Display Current Date

#!/bin/bash

echo "Current date and time: $(date)"

📝 Uses the date command to show current system time.

--------------------------------------

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

--------------------------

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

-----------------------------------

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
bash
CopyEdit
#!/bin/bash
read -p "Enter filename to backup: " file
cp "$file" "$file.bak"
echo "Backup created as $file.bak"

📝 Creates a .bak copy of a file.
