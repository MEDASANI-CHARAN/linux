# Linux commands

---

## Basic Commands
- `pwd` -> present working directory
- `cd` -> change directory
- `ssh-keygen --help` -> usage of this command
- `uname` -> kernal name
- `uname --help` -> indetailed kernal name
- `man uname` -> manual uname
- `history` -> the data you searched
- `cd /` -> root directory
- `cd <folder-name>` -> to enter into folder
- `cat <file-name>` -> to read the file
- `cat > <file-name>` -> overwrite/replace the content in file
- `cat >> <file-name>` -> append the data in file

---

## List
- `ls` -> list of subdirectories
- `ls --help` -> list information
- `ls -l` -> long listing format
- `ls -lr` -> reverse alphabetical order
- `ls -lt` -> latest files or folders
- `ls -ltr` -> starts from old files
- `ls -ltrh` -> convert into kilo bites (h means human readable)
- `ls -la` -> all files or folders including hidden

---

## File
- `touch <file-name>` -> create a file

---

## Folder (or) Directory
- `mkdir <folder/directory-name>` -> create folder/directory

---

## Remove (or) Delete
- `rm <file-name>` -> to delete the file
- `rm -r <folder/directory-name>` -> delete folder/directory
- `rm -rf <folder/directory-name>` -> delete folder/directory forcely
- `rmdir <folder/directory-name>` -> delete only empty folder/directory

---

## Copy & Move
- `cp <source-file> <destination-path>` -> copy file to destination path
- `cp -r <source-directory> <destination-path>` -> copy directory to destination directory we have mention recursive
- `mv <source-path> <new-name>` -> it will rename the file

---

## Search
- `grep <word-to-search> <file-name>` -> to find words
- `grep -i <word-to-search> <File-name>` -> if we give mixed uppercase/lowercase in file we have to mention -i i.e case insentive

### Piping
- `cat <file-name> | grep <word-to-search>` -> piping
- `cat <file-name> | grep -i <word-to-search>` -> piping with case sencitive

---

## wget & curl
- `wget <url>` -> download the files, folders or softwares into linux servers (webget)
- `curl <url>` -> display the text directly into the terminal

---

## Print Text
- `echo <text>` -> to print the data

---

## Cut and awk
- `echo <url> | cut -d / -f<number>` -> cut command is used to to get the fragments of a text usig delimiter
- `echo <url> | cut -d / -f1- --output-delimiter=$'\n'` -> To see all fragments
- `echo <url> | cut -d / -f1-2` -> To see forst 2 fragments =>(-f means field & -d means delimiter)
- `echo <url> | awk -F "/" '{print $<numner>F}'` -> awk command is used to text processing.. generraly used to devide the test in column format
- `echo <url> | awk -F "/" '{print $NF}'` (-F means Field Separator)
- `echo <url> | awk -F "/" '{print NF}'` -> Count how many fields exist
- `echo <url> | awk -F ":" '{print $1F}'` -> seperated by colon
- `echo <url> | awk -F ":" '{print $NF}'`
- `awk -F ":" '{print $1F}' <file-name>` -> To find first names in a list
- `awk -F ":" '{print $1F,$3F}' <file-name>`

### Difference b/w cut and awk
**cut:**
- Works fast, but limited (can’t do calculations, filtering, conditions)
```bash
echo "name,age,city" | cut -d, -f2
```
**awk:**
- Can apply conditions, loops, calculations, formatting
```bash
echo "name,age,city" | awk -F, '{print $2}'
```
---

## Head & Tail
- `head <file-name>` -> gives first 10 lines of the file
- `tail <file-name>` -> last 10 lines of the file
- `head -n <number> <file-name>` -> first 2 lines of the file
- `tail -n <number> <file-name>` -> last 2 lines of the file

---

## Find
- `find <where-to-search> -name <file-name>` -> To find the file

**Examples:**
`sudo find / -name <users>` -> To find the name in root directory  
`find . -name "users"` -> To find the name in current directory  
`find . -name "*se*"`

---

## CRUD -> Create, Read, Update, Delete
**CRUD example:**
- when you signup to facebook, gmail etc.. - create
- when you login to facebook, gmail etc.. - read
- when you update your profile in facebook, gmail etc.. - update
- when you delete your profile in facebook, gmail etc.. - delete
