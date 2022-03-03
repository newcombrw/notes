Tricks:  
ctrl+R === the "reverse i search" search feature. you can also add a comment and search by comment  
for very long commands, you can use this to use the command again  
sudo !! === run the last command you tried, but this time with sudo  


Directories:  
mkdir -p /{}/{}/{} === even if the folder doesnt exist yet, create it and nest the next directory with -p  
cd - === go back to your previous directory  

File Manip:  
curl cht.sh/<command> === list examples of the command <command>  
explainshell.com === paste a command in here and get an explaination of the command  

which - get the absolute path of the given command  
whereis - get the absolute file path of a command (including all hits)  
whatis - get the man page synopsis of a command  

egrep -v "exlude this" === return every line that doesnt contain the matched text  
file 



.  
.  
.  
.  
1.1: mkdir $HOME/11{23,34,45,56}  
1.2: touch $HOME/1123/{1,2,3,4,5}.txt; touch $HOME/1123/{6,7,8,9}\~.txt  
1.3: find $HOME/1123 -name *.txt | grep -v "*\~\*"
2: find $HOME/1123 -name \*.txt \\! -name '\*\~\*' -exec cp $HOME/CUT {} \;  
3: find /lib -empty -printf "%i %f\n"  
4: find / -inum 999 -printf "%f\n"  
5:  
```bash
#!/bin/bash
ls -l -not -type d .$1 | grep -v "names.txt" > $HOME/CUT/names.txt
```
  
