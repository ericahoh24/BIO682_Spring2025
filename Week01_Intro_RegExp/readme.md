# Class 1 - Jan. 17th 2025
- In this first class we will:
    - Discuss the syllabus and course organization/expectations
    - Troubleshoot computer setup problems
    - Learn to use regular expressions to edit plain text files

### Required Reading (**Must be completed ahead of time**)
Practical Computing for Biologists, Chapters 1-3

### Prep for next class

1. Open your command line interface and type this command followed by 'Enter':
```echo $SHELL```

If the reponse is not "/bin/bash" or "/bin/zsh", let me know. 

### Assignment

1. Go to [RegexOne](https://regexone.com/) and complete the 15 (and 1/2) lesson tutorial. This website provides a nice interactive interface for playing with regular expressions.
    - Although the interface will allow you to only match a portion of each line, when possible, I encourage you to write expressions that match the entirety of each line. 
    - **Keep track of your solutions in the table provided in the Assignment Answer Sheet.**

2. We will now start using the text editor on your computer to use regular expressions to edit text files. 
    1. Open "filenames.txt" in your text editor. This file contains a list of filenames.
    2. Oops, looks like there's an extra period in each file name, and the file extension has mistakenly been capitalized. Use a single find/replace query to convert ```..Fasta``` to ```.fasta```. **Record your find/replace query in the Assignment Answer Sheet.**
    3. Next, let's use regular expressions to convert these file names into shell commands that will count the number of sequences present in each file. We will learn more about shell scripting in the coming weeks, but to do this all you need to do is add ```grep -c '>' ``` onto the beginning of each line that contains a file name (make sure there is a space between the command and each file name). **Please use a single find/replace query and record it in the Assignment Answer Sheet.**
    4. Now let's add file paths onto the beginning of these filenames so that the commands can be run from any location on your computer. We'll talk more about file paths next week, but they provide instructions about where to find the files on your computer. Use a single find/replace query to add ```/Users/fakeuser/Documents/sequences/``` just prior to each file name (and after the shell command you added in the previous step). **Record your find/replace query in the Assignment Answer Sheet.**
    5. **Upload final re-formatted text file to Canvas along with Assignment Answer Sheet.**

3. Open "HastingsBirdList\_2007.txt" in your text editor. This file contains tab-delimited information about bird species cited in the Hastings Park Conservancy in Vancouver, BC.
    1. Design a **single search and replace query** that utilizes regular expressions to reformat **every** line to match the following:
    ```Genus\tspecies\tG. species\tCommon Name\tStatus```
    "Status" is the column with a categorical variable including "Casual", "Rare Visitor", etc. Make sure to remove the "\*" character from the beginning of the Status category, if present. **Record the find/replace query in the Assignment answer sheet.** (Tip: Copy and paste reformatted text into Excel to double check your solution.)
    2. **Upload re-formatted file to Canvas along with Assignment Answer Sheet.**
    
## Extra fun

Explore for "extra credit" or in the event that you finish all of the other exercises.

[RegexOne Problems](https://regexone.com/problem/matching_decimal_numbers)

[Regex Crossword](https://regexcrossword.com/)

Copyright (C) 2025  Jason Ladner

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.



