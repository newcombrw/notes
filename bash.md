
1: mkdir, touch, ls, rm, rmdir, cp, mv, cat, more, less, find, egrep/grep, brace expression, ps, kill, killall, cut, command chaining operators, output redirection
2: awk, sort, uniq, conditionals, if statements, aliases, sed 
3: variables, command substitution, builtin variables, functions 
4: for, while, until loops


  ##SHELL COMMANDS
```mkdir```
```touch```
```ls```
```rm```
```rmdir```
```cp```
```mv```
```more``` ```head``` ```less``` ```tail``` ```cat```
```find```
```egrep```
```ps```
```kill/pkill/killall```
```cut```
```awk```
```sort```
```uniq```
```sed```

  ##SCRIPTING CONCEPTS  
__Variable Declaration__  

__Conditionals__  

__Command Chain Operators__  

__Loops__  
 ```bash
  for THING in my list of things this is a list
  do
    echo $THING
  done
  
  #iterate over array variable
  names='Stan Kyle Cartman'
  for name in $names
  do
  echo $name
  done
  
  #range loop
  for value in {1..5}
  do
  echo $value
  done
  
  for value in {10..1}
  do
  echo $value
  sleep 1
  done
  echo "Blast off"
  
  #counter loop
  for ((x=0 ; x<=5 ; x++))
  do
  echo "\$x equals $x"
  (( i++ )) #another way to increment i when using the c-style for loop
  done
  
  start=1
  end=10
  for ((i=start; i<=end; i++))
  do
  echo $i
  done
  
  for i in $(ls *.txt) #you can create a list from a command, which you can iterate through
  
  
  ```  
__Command Substitution, Brace Expansion__  
__TRICKS__  
ctrl+R === the "reverse i search" search feature. you can also add a comment and search by comment  
for very long commands, you can use this to use the command again  
sudo !! === run the last command you tried, but this time with sudo  

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

