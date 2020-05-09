# Programming Basics questions

## Computer science

### Data structures

#### What is the purpose of a list (array in some programming languages) data structure? Name some methods of it!
The purpose of a list/array, is to store different variables, close to each other. Like names.
Methods:
Append method = next element becomes the list's member
Count method = counts number of elements in list
Extend method = same as append, but with multiple elements at once
Insert method = like append, except instead of putting to the end, inserts to the given index
Index method = returns index of something that is in list. if present multiple times returns first exception.
#### What is the difference between a list/array and a set?
While lists'/arrays' elements can be changed even after declaration, set's can't. Once declared, they stay the same. Also, multiplications. In lists/arrays they can happen. In sets they will be deleted uppon occurence.
#### What is the purpose and methods of a dictionary/map data structure?
Purpose is storing key-value pairs. Storing values, with easier way to index, instead of just numbers. Like phone numbers to store, based on their owners' names.
Methods:
Get method = returns value based on key or None if it doesn't exist.
Update method = much like append in lists. Adds several items to the dictionary once.
Keys method = returns the keys of the dictionary.
Values method =  returns the values of the dictionary.
Items method = returns both the keys and values of the dictionary.
### Algorithms

#### Fibonacci sequences. Write a method (or pseudo code), that generates the Fibonacci sequences.
We need a list. It's first 2 elements, being 0 and 1. The next element always will be the sum of the 2 latest element. The sum happens 5-10 times. Done.
#### How do you find a max value in a list/array if you can’t use any built-in functions?
You go through the list/array once. Each time you go through an element, check if that element is higher than the last higher, which is stored in a variable. Once done the variable contains the highest number.
#### How do you find the average of values in a list/array if you can’t use any built-in functions?
You go through the list/array once. While going through it count the length of it, and sum the values. Doing both in seperate variables. Once done, divide the sum by the count. The outcome is the avarage.
#### What do we call an *in-place* sort?
Sorting a variable, in-place. Meaning not giving it's sorted outcome to any other variable at all.
#### Explain an algorithm which sorts a list!
The algorith goes through the list, as many times as the length of the list is. Each time, if check for the element, that is highest, but not higher than the one, that was last time highest. First time of course will look for highest one. And put it before the highest one. This is how to sort in descending order.
### Programming paradigms - procedural

#### What is the call stack?
#### What is “Stack overflow”?
#### What are the main parts of a function?

### Programming languages - Python  
#### How do you use a dictionary in Python?
#### What does it mean that an object is immutable in Python?
#### What is conditional expression in Python?
#### What are different types of arguments in Python?
#### What is variable shadowing? (context: variable scope)
#### What can happen if you try to delete/drop/add an item from a List, while you are iterating over it in Python?
#### What is the "golden rule" of variable scoping in Python (context: LEGB)? What is the lifetime of variables?
#### If you need to access the iterator variable after a for loop, how would you do it in Python?
#### What type of elements can a list contain in Python?
#### What is slice operator in Python and how to use?
#### What arithmetic operators (+,*,-,/) can be used on lists in Python? What do they do?
#### What is the purpose of the in and not in membership operators in Python?
#### What does the + operator mean when used with strings in Python?
#### Explain f strings in Python?
#### Name 4 iterable types in Python!
#### What is the difference between list/set/dictionary comprehension and a generator expression in Python?
#### Does the order of the function definitions matter in Python? Why?
#### What does unpacking mean in Python?
#### What happens when you try to assign the result of a function which has no return statement to a variable in Python?

## Software engineering

### Debugging

#### What techniques can you use while debugging a program in Python?
#### What does step over, step into and step out mean while using the debugger?
#### How can you start to debug a program from a certain line using the debugger?

### Version control

#### What are the advantages of using a version control system?
#### What is the difference between the working directory, the staging area and the repository in git?
#### What are remote repositories in git?
#### Why does a merge conflict occur?
#### Through what series of commands could you put a new file into a remote repository connected to your existing local repository?
#### What does it mean atomic commits and descriptive commit messages?
#### What’s the difference between git and GitHub?

## Software design

### Clean code

#### What does clean code mean?
#### What steps do we usually do during a clean code refactoring?

### Error handling

#### What is exception handling?
#### What are the basics of exception handling in Python?
#### In which case should we catch an exception? Why?
#### What can/should we do with an exception in the ‘except’ block?
#### What does the else and finally statement do in a try-except block in Python?

## Software Development Methodologies

#### What is the main goal of a retrospective meeting?

## Programming environment

### Unix

#### What is UNIX and what is Linux?
#### What do we call the shell in Linux?
#### What does root means in a Linux environment?
#### How do you access your personal files in Linux?
#### How can you install an application in Linux?
#### What is package management in Linux, what are repositories?
#### How do you navigate in the filesystem with the command line?
#### What does the following commands do: mkdir, rm, cat, cp, touch?
#### How can you look up what does a command do in Linux if you have no internet connection?
#### What does the following commands do: head, tail, more, less?
#### How do you download a file from internet using the terminal?
