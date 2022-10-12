# MobileAppLocalizer

This is a utility written in Python3. It can be used to generate localization files for iOS & Android.

# Why ?
When team works on iOS and Android apps on different code bases, it is redundant and tedious work to update the strings during development lifecyle, seperately whenever there is a new change. Also, it causes mismatch and incosistency many times.

# What it does ?
This utility reads the strings (keys & values) from localization.xls files, create seperate localizable files for iOS and Android (.strings & .xml respectively) and add all localized strings in files which will be used by mobile apps. 

# How to use this ?
You need to have python3 and pip3 installed in ur machine. If it is not installed, please install both of them. Also install pandas(package to read excel) using pip3 in your dev machine.
To test this utility, 
  1. Checkout this project
  2. Go to project directory in terminal
  3. Run the command -> python3 Localize.py
  
  You will see Localization folder generated for iOS containing .lproj folders and files. Also it will generate res folder with strings.xml for all three languages.
  
# How to customize and use for any project ?
1. Open Localization.xlsx file and add keys & values for each language.
2. I have used dirName = os.getcwd() to get project's current directory. Just change this path for Localization.xlsx file, the iOS and Android project directory path where you want it to be generated and run the code.





