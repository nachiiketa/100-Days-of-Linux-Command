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


