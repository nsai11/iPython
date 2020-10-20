# iPython
iPython, short for Indian Python is an attempt to run python in Indian and devanagiri languages.

# Inspiration
http://www.chinesepython.org/home.html

# Usecase
This project aims to help children and people with less exposure to English, transition better to CPython, the official Python.

# Path 1 (current track)
1. Need to create a mapping script that maps Hindi keywords to their english counterpart
2. Write a script that includes this mapping to parse a given program
3. The above script needs to parse the program, tokenize hindi words and build an english program.
4. The english program would run and deliver the output back to the hindi program

# Path 2(Suitable track)
1. Modify grammar.c 
2. Modify pythonrun.c to enable hindi version of 'from xx import xx'
3. traverse Objects/ to make builtin types/objects more friendly
   by adding ª°©˙, ¶W∫Ÿ ..
4. add hindi function alias to built in methods of stringobject, 
   fileobject
5. traverse Python/compile.c ceval.c exceptions.c errors.c modsupport.c ...
   to make more hindi messages there
6. modify Python/bltinmodules.c and give chinese name to builtin functions 
7. edit setup.py to cope for chinese version of modules
8. copy english module files and rename to something else, 
   work on those files to replace functions, labels to chinese
9. compile both versions of modules in and check
10. create hindi version of the file in /Lib
  
