# Command-Line Coda

Command-Line Coda is a script for [Panic](http://panic.com)'s Coda. It allows you to open files in Coda from the command line.

## Usage

	coda [a list of files or directories you want to open]

	coda myfile.txt                   # coda creates files if they don't exist
	coda somedir                      # if you specify a directory, coda will open all files in that directory
	coda file1.txt file2.txt somedir3 # you can open multiple files

## Install

	gem install coda

## Updates (chrisphenry)

## Coda 2 Support
This version of Command Line Coda has been specifically updated to support Coda 2 by default.
>> the need for a .bash_profile or modification thereof is not required if Coda 2 is living in your User/Applications
folder.
>> direct bin/coda file is hardcoded: `CODAPATH = ENV['CODAPATH'] || "/Applications/Coda 2.app"`

## Setting Coda's path (optional)
>> by deafult we assume the location of Coda 2 is the OS default: `/User/Applications/Coda 2.app`
>> to override the default path do the following:

#### Step 1
Open or Create the `.bash_profile` file which belongs here (home folder): `~/` -if it doesn't exist, you must create it -the "." is required in the filename. 
#### Step 2
Add the line: `CODAPATH="Path/Coda 2.app"` exactly as shown (with quotes around the path itself) + save.

Updated by [Chris Henry](https://github.com/chrisphenry). Can't see it breaking your computer!

Written by [Aditya Bhargava](http://adit.io). No warranty is implied, use at your own risk.
