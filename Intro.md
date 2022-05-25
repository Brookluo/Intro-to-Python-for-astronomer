# This is an introduction to Python for astronomers (Yes, you!)

<img src="./images/Uncle_Sam.png" alt="sam" width=100/>

## A brief history of Python

Python was invented by Guido van Rossum in late 80s. Python has three generations, Python 1, 2, and 3. Python 3 is the most recent version, and is the only one currently supported and recommended by the Python foundation. There are many fundamental differences between Python 2 and 3, so if you are using Python 2, think twice and turn away! 

Python is a __dynamically-typed, interpreted__ general-purpose programming language. Dynamically-typed means the type of an object is assigned during runtime of the program. Interpreted means Python is executed with the help of another program: an interpreter. The interpreter translates lines of python code into another machine language (assembly) that a computer can understand and execute.


Bonus: why does Python logo look like this one? the python ecosystem? 

![snake](images/download.jpg)

## Features of python

Python is very versatile and can achieve almost all programming tasks desired by scientists and engineers, if performance and security are not concerns. Python has been widely used in astronomy for data reduction, analysis, plotting, and more. In this tutorial, I will talk about the basic features and functionality of python but moreover my intention is to help you understand the big picture of programming: read other people's code, read documents of modules, code your tasks, debug them, and communicate your code and results with your peers.

Let's dive in!

## Python interactive shell

An python interpreter should have been installed on all department computers, and the default version is `3.6.13`. It is good for now. 
We will come back later and talk about how to manage your environment and switch between different versions of python. We can check python version and start python interactive shell or **REPL** (Read, Evaluate, Print, Loop) by 

```shell
[brook@shoshone ~]$ bash
(base) bash-4.4$ python --version
Python 3.6.13 :: Anaconda, Inc.
(base) bash-4.4$ python
Python 3.6.13 |Anaconda, Inc.| (default, Feb 23 2021, 21:15:04)
[GCC 7.3.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>>
```
This is the starting point of using Python. Note that the default shell for our department is csh, so we have to type `bash` to change to bash shell. We can now type commands to do some simple tasks.

```python
>>> print("hello, world!")
hello, world!
>>> a = 100
>>> print(a)
100
>>> c = 2
>>> a + c
102
>>>
```

To exit the python REPL, we need to use `exit()` or hit `ctrl + D`. If your programming task is simple, you can just use the python REPL as a super TI-89 scientific calculator. However, there are many more times, the programming task is very complex, and cannot be achieved with just a few lines of code. We then need a file to store all the commands. This file is python script, whose file name suffix is `.py`. Let's put the commands above into a file called `test.py`

```python
print("hello, world!")
a = 100
print(a)
c = 2
a + c
```

The python script can be run with

```bash
(base) bash-4.4$ python test.py
hello, world!
100
```

Wait, it looks like we are missing something in the result? Why was it missing? 

The python REPL is an interactive shell environment, just as the name indicates, will print the result automatically if there is no assignment, etc. That is a very useful feature if we want to explore some new data set and check the result.
Sometimes, we want to take advantage of the interactive feature of the python REPL, and also save the commands for future use. What should we use? 

(Jupyter notebook!)



