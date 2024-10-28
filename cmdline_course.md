---
layout: default
---


# Command-Line Course

This course introduces the fundamentals of using the command-line interface (CLI). Over several weeks, we covered topics ranging from basic navigation to more advanced shell scripting.

## Week 1: Introduction to Command Line Environments
In the first week of the course we got acquainted with such environments as Ubuntu and Linux. We got acquainted with the nano editor, learned how to create new files and edit old ones. We also learned the most basic Linux command line commands, such as:

### Example Code
```bash
# List all files in a directory
ls
# Overwrite file1 to file2
mv file1 file2
# Copy file1
cp file1 file2
# Make a new direction
mkdir
# Write and addit files
nano file
```

## Week 2: Navigating a UNIX System
The second week focused on more advanced file and directory operations. We learned how to copy and delete directories, compress files and directories using gzip and tar, and change file permissions. We also explored process management, running tasks in the background, connecting to remote servers, and transferring files using scp.

### Example Code
```bash
# Remove directory
rmdir
# Kill processes
kill
# Connect to remote servers
ssh
```

## Week 3: Basic Corpus Processing
In the third week, the emphasis was on working with text files. We learned about different encoding systems and how to convert files between them. We practiced sorting lines in a file, removing duplicates, working with text columns, and extracting data. Additionally, we learned how to search for patterns in files and save results. These skills are particularly useful for analyzing and transforming large amounts of text data.

Encoding systems we learned:
- ASCII, 
- Latin-1,
- UTF-8.

### Example Code
```bash
# Transform windows end of lines to unix end of line
dos2unix
# Replace characters ( # with \n)
tr '#' '\n'
# Sort the lines
sort
# Keep only uniq lines
uniq
```

## Week 4: Advanced Corpus Processing
The fourth week was dedicated to more in-depth text editing using sed and regular expressions. We learned how to delete lines, find and replace patterns, and chain commands using pipelines. We also covered generating frequency lists and creating n-grams from text files. These skills allowed us to automate tasks related to text processing.

### Example code
```bash
# Dellite lines with sed
sed //d
# Replace patterns with sed (X.# with X. for example)  
sed -E s/([IVX][.])#/\1/g
```

## Week 5: Scripting and Configuration Files
In the fifth week, we began writing simple scripts to automate tasks. We learned how to use command-line parameters in scripts, apply conditional statements, and perform command substitution. We also explored how to modify and save environment variables in .bashrc or .bash_profile files to create a comfortable working environment in the terminal.

### Example Script
```bash
#! /bin/bash


# script: comparative_step1.sh
# author: Sofia Gruk

# This script takes an English adjective and prints its comparative form.

#If the number of arguments is not 1, the script returns an error and shows how to use it correctly.
if [ $# -ne 1 ]
then
   echo 'ERROR: One argument required!'
   echo './comparative_step1.sh input_adjective'
   exit 1
fi

#If the argument does not end in a vowel, the script returns an error and instructions for use. Otherwise, it substitutes ER for the argument and outputs it.
adjective=$1
if [[ "$adjective" =~ [^aeiouyAEIOUY]$ ]];
then
   comparative="${adjective}er"
else
   echo 'ERROR: The adjective must end in a consonant!'
   echo './comparative_step1.sh input_adjective'
   exit 1
fi

echo "$comparative"
```

## Week 6: Installing and Running Programs
The sixth week covered software installation through the command line. We learned how to install packages using apt-get, brew, and pip, as well as create Python virtual environments to manage packages. Additionally, we learned how to write and run Makefiles to simplify project workflows. These skills made it easier to manage the programming environment and streamline the development process.

### Example Code
```bash
# Become a root user for one command
sudo #command
# Download a packege
apt-get
# Use python virtual environment
python -m venv
```

## Week 7: Version Control

In the seventh week, we were introduced to the version control system Git. We learned how to create local and remote repositories, add files, commit changes, and push them to GitHub. We also explored branch management and merging branches with the main branch. Version control is essential for efficiently managing projects, especially in a team setting.

### Example Code
```bash
# Clone a remote repo
git clone <url>
# Add all untracked files, that were updated
git add -A
# Commit changes with description
git commit -m "<description>"
# Push updated files from origin to master branch
git push origin master
# Make a new branch
git checkout -b <branch_name>
```

## Week 8: Final Project
The final week of the course was dedicated to a project where we applied all the skills they had learned. This allowed them to consolidate their knowledge of command-line usage, scripting, and Git, resulting in a complete project ready for deployment and publication on GitHub Pages.

### Example Code
```bash
# Install build-essential package and ffi development library
sudo apt-get install build-essential libffi-dev
# Install ruby using apt-get
sudo apt-get install ruby ruby-dev
```

# Course Comprehension Сhart

    | Week № | Score |
    |--------|-------|
    | Week 1 |  10/10|
    | Week 2 |   9/10|
    | Week 3 |   8/10|
    | Week 4 |   9/10|
    | Week 5 |   9/10|
    | Week 6 |  10/10|  
    | Week 7 |  10/10|

# General Feedback
As you can see from my Course Comprehension Chart, I found it to be fairly easy. However, I can confidently say that it is very useful and provides the basic knowledge that everyone should know in the technology field.
    
