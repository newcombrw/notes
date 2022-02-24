__PYTHON__  
__F'NZ__
  syntax:
  ```python 
  def myFunction(<params...>):
    return val
  ```
  defines a function with any parameters and returns a value.
  
  __SCOPE__
  objects, variables, or functions defined anywhere in a script is considered a global variable
  if these are defined within a function, they are local variables
  you can not change global variables from within functions without prepending the ```global``` keyword to the declaration
  
  __LOOPS__
  syntax:
  ```python
  while <condition>:
    <do something>
  for var in <set>:
    <do something>
  ```
  for loops iterate over a set. for an arbitrary iterator i, you can use range(noninclusivelimit) to iterate with an increasing iterator i:
  ```python
  #print 1 to 9
  i = 1
  for i in range(10):
    print(i)
  ```
  
  __RANGE/ STRINGSPLICING__
  using ```range(start, stop, step)```: follow the mneumonic START, STOP, STEP
  START: where to start, inclusive; STOP: where to stop, non-inclusive, STEP: add by this much every step
  ```
  range(0,10,2) === [0, 2, 4, 6, 8]
  range(5,0,-1) === [5, 4, 3, 2, 1]
  ```
  
  string splicing syntax: ```myIterable[START:STOP:STEP]``` a shorthand for for-range loops. Allows leaving START/STOP blank.
  ```python
  myStr = "hello"
  myStr[0:2]  === he
  myStr[::-1] === olleh <displays the string/list in reverse>
  myStr[:-1]  === hell <displays the list/string without including te last element>
  ```
  
  
  __USEFUL FUNCTIONS__  
  ```ord(character)          ```=== get the ordinal value (decimal representation) of a single string character  
  ```format(integer, '0>8b') ```=== format a number to be represented as binary without a binary indicator (no 0b010101, 00010101 instead)  
  ```int(to convert, base)   ```=== specify a base when converting a string (or other type) to an integer  
  ```chr(integer)            ```=== interprets an integer as an ordinal value, and represents it as the ASCII value of the number  
  ```len(str) or len(list)   ```=== gets the length of a string in characters, or the length of a list in elements
  
  __FILEIO__  
  use ```open(strName)``` to open a file. this returns a file pointer object. use ```filePointerObject.close()``` to close the file.  
  shorthand open/close:  
  ```python
  with open(strName, 'rwb') as fp:
    #work on the file here
    fp.read() === read all the lines from the file as a string. you can specify how many bytes to read (fp.read(value))
    fp.write("string to write") === write to the file. replace everything else. no newline character
    fp.readlines() === reads the whole file as a list of strings. each element is delimited by a new line
    fp.writelines(['str1', 'str2']) === same as write, but inserts everything as the list. you need to add new lines as before
  ```
  
