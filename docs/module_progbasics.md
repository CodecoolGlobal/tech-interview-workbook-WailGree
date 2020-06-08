# Programming Basics questions

## Computer science

### Data structures

#### What is the purpose of a list (array in some programming languages) data structure? Name some methods of it!

*The purpose of a list/array, is to store different values, close to each other. Like names.*

Methods:
1. **list():** *creates a list in Python.* **list([iterable])**
2. **append():** *Add a single element to the end of the list.* **list.append(item)**
3. **extend():** *Add Elements of a List to Another List.* **list1.extend(list2)**
4. **insert():** *Inserts Element to The List.*- **list.insert(index, element)**
5. **remove():** *Removes item from the list.* **list.remove(element)**
6. **clear():** *Removes all Items from the List.* **list.clear()**
7. **index():** *returns smallest index of element in list.* **list.index(element)**
#### What is the difference between a list/array and a set?
*While lists'/arrays' elements can be changed even after declaration, set's can't. Once declared, they stay the same. Also, multiplications. In lists/arrays they can happen. In sets they will be deleted uppon occurence.*
#### What is the purpose and methods of a dictionary/map data structure?
*Purpose is storing key-value pairs. Storing values, with easier way to index, instead of just numbers. Like phone numbers to store, based on their owners' names.*

Methods:
1. **dict():** *Creates a dictionary in Python.* **dict({key: value})**
2. **get():** *Returns value based on key or None if it doesn't exist.* **dict.get(key)**
3. **update():** * Much like append in lists. Adds several items to the dictionary once. Also can change already existing value.*
4. **keys()** *Returns the keys of the dictionary.* **dict.keys()**
Values method =  returns the values of the dictionary.
Items method = returns both the keys and values of the dictionary.
### Algorithms

#### Fibonacci sequences. Write a method (or pseudo code), that generates the Fibonacci sequences.

[source](https://www.mathsisfun.com/numbers/fibonacci-sequence.html)
[source](https://www.geeksforgeeks.org/python-program-for-program-for-fibonacci-numbers-2/)

xn = xn−1 + xn−2

```Python
def Fibonacci(n):
    if n<0:
        print("Incorrect input")
    elif n==0:
        return 0
    elif n==1:
        return 1
    else:
        return Fibonacci(n-1)+Fibonacci(n-2)
```

#### How do you find a max value in a list/array if you can’t use any built-in functions?

1. *sort method:*
*You go through the list/array once. Each time you go through an element, check if that element is higher 
than the last higher, which is stored in a variable. Once done the variable contains the highest number.*


```Python
def find_max():
    lst = [1, 9, 7, 3, - 2]
    max = 0
    for i in lst:
        if i > max:
            max = i
    return max
```

2. *print the last element  in a list*

#### How do you find the average of values in a list/array if you can’t use any built-in functions?
You go through the list/array once. While going through it count the length of it, and sum the values. Doing both in seperate variables. Once done, divide the sum by the count. The outcome is the avarage.

1. *add elements to eachother*
2. *count them with a variable*
3. *add  divide them by a variable*

```Python
def find_avg():
    lst = [1, 9, 7, 3, - 2]
    count = 0
    sum = 0
    for i in lst:
        count += 1
        sum = sum  + i
    avg = sum/count
    return avg
```


#### What do we call an *in-place* sort?

*Sorting a list, in-place. Meaning not giving it's sorted outcome to any other variable at all, only modifying the order of the elements within the list.*

#### Explain an algorithm which sorts a list!

**Bubble sort:**
*The algorith goes through the list, as many times as the length of the list is. Each time, check adjacent elements, if second is higher than first. If so, swap them. Result, highest number as first element, then second lowest, then thirds, etc. This is how to sort in descending order.

### Programming paradigms - procedural

#### What is the call stack?

*It's a data structure that stores information. The program uses it to keep track of method calls.*

![pic](https://res.cloudinary.com/practicaldev/image/fetch/s--s1Qbl8Gf--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/mwcwre09s12vqa3gvl7a.png)

#### What is “Stack overflow”?

**An error type.**

*In softwarem a stack overflow occurs if the call stack pointer exceeds the stack bound. The call stack may consist of a limited amount of address space, oftendetermined at the start of the program. The size of the call stack depends on many factors, including the programming language, machine architecture, multi-threading, and amount of available memory. When a program attempts to use more space than is available on the call stack , the stack is said to overflow, typically resulting in a program crash. Recursive function never quit.*

*In short, if we run out of space, the program will send this error.*

#### What are the main parts of a function?

```Python
def random(arg1, arg2): # function signature(function name,paramater list)
    multiply = arg1+ arg2 # function body
    return multiply
```

### Programming languages - Python  

#### How do you use a dictionary in Python?

[source](https://www.w3schools.com/python/python_dictionaries.asp)

*A dictionary is a collection which is unorered, changable and indexed. In Python dictionaries are written in curly brackets, and they have keys and values. dict_name = {key:, ... keyN:valueN}*

```Python
#declaring
dictionary = {'a':2, 'b'3, 'c':4}
#printing the dict
print(dictionary)
#getting the value of a key and store it
x = dictionary.get('a')
# variable x becomes equal to 2
```

#### What does it mean that an object is immutable in Python?

*These are of in-built types like int, float, bool, string, unicode, tuple.*
*An immutable object can't be changed after it is created.*

#### What is conditional expression in Python?

[source](https://en.wikipedia.org/wiki/%3F:#Python)

*Ternary operators also known as conditional expressions are operators that evaluate something based on a condition being true or false.*

\<expression1> if \<condition> else \<expression2>

<value_if_true> if <statement> else <value_if_false>

'Yes' if fruit == 'Apple' else 'No'

#### What are different types of arguments in Python?

[source](http://www.trytoprogram.com/python-programming/python-function-arguments/)

1. **Default Arguments:** *def sum(a=4, b=2):*
2. **Keyword Arguments:** *def print_name(name1, name2): print_name(name2 = 'John', name1 = 'Gary')*
3. **Variable-length Arguments:** *def display(\*name, \*\*address): display('john','Mary','Nina',John='LA',Mary='NY',Nina='DC')*
*(args) - Arguents,  **(KWargs) (Key Word Arguments)**

#### What is variable shadowing? (context: variable scope)

*In computer programming, variable shadowing occurs when a variable declared within a certain scope (decision block, method, or inner class) has the same name as a variable declared in an outer scope. At the level of identifiers (names, rather than variables), this is known as name masking.*

*(t's defined as when a variable "hides" another variable with the same name. So, when variable shadowing occurs, there are two or more variables with the same name, and their definitions are dependent on their scope (meaning their values may be different depending upon scope).)*

#### What can happen if you try to delete/drop/add an item from a List, while you are iterating over it in Python?

[source](https://www.quora.com/In-Python-why-cant-you-remove-elements-from-a-list-with-a-for-loop-but-you-can-with-a-while-loop)

*An error will ocurr.*

*If the error wouldn't occur the following could happen:*

1. *When we delete an item from the list the for loop will skip some elements, because we changed the list(indexing).*

2. *When we add an item  to the list the for loop will be forever running.*

#### What is the "golden rule" of variable scoping in Python (context: LEGB)? What is the lifetime of variables?

[source](https://www.geeksforgeeks.org/scope-resolution-in-python-legb-rule/)

*In Python, the LEGB rule is used to decide the order in whiceh the namespaces are to be searched for scope resolution.
The scopes are listed below interms of hierarchy (highest to lowest/narrowest to broadest):*

1. **Local(L):** *Defined inside function/class*
2. **Enclosed(E):** *Defined inside enclosing functions(Nested function concept)*
3. **Global(G):** *Defined at the uppermost/global level*.
4. **Built-in(B):** *Reserved names in Python builtin modules*

#### If you need to access the iterator variable after a for loop, how would you do it in Python?

*If you need it after a loop, you store it in another variable, INSIDE the foor loop. When it ends you can use the new variable afterwards.*

#### What type of elements can a list contain in Python?

Each item in a python list can be of any data type.
*fe: string, numbers, list, tuple, dict*

#### What is slice operator in Python and how to use?

[source](https://www.w3schools.com/python/ref_func_slice.asp)

The **slice()** function returns a slice object.
*slice(start, end, step)*

```Python
a[start:stop:step]
a[slice(start, stop, step)]
```

**list slicing:**
list:  listname[0:2] [:4] [1:-1] [:]

#### What arithmetic operators (+,*,-,/) can be used on lists in Python? What do they do?

[source](https://www.tutorialgateway.org/python-program-to-perform-arithmetic-operations-on-lists/)

```Python
NumList1 = [10, 20, 30]
NumList2 = [5, 2, 3]
add_lists = []
add = []
sub = []
multi = []
div = []
mod = []
expo = []

add_lists = NumList1 + NumList2

for j in range(3):
    add.append( NumList1[j] + NumList2[j])
    sub.append( NumList1[j] - NumList2[j])
    multi.append( NumList1[j] * NumList2[j])
    div.append( NumList1[j] / NumList2[j])
    mod.append( NumList1[j] % NumList2[j])
    expo.append( NumList1[j] ** NumList2[j])

print("\The List Items after Merging = ", add_lists)
print("\nThe List Items after Addition =  ", add)
print("The List Items after Subtraction =  ", sub)
print("The List Items after Multiplication =  ", multi)
print("The List Items after Division =  ", div)
print("The List Items after Modulus =  ", mod)
print("The List Items after Exponent =  ", expo)

output:
The List Items after Merging =   [10, 20, 30]
The List Items after Addition =   [15, 22, 33]
The List Items after Subtraction =   [5, 18, 27]
The List Items after Multiplication =   [50, 40, 90]
The List Items after Division =   [2.0, 10.0, 10.0]
The List Items after Modulus =   [0, 0, 0]
The List Items after Exponent =   [100000, 400, 27000]
```

#### What is the purpose of the in and not in membership operators in Python?

[source](https://www.geeksforgeeks.org/python-membership-identity-operators-not-not/)

Membership operators are operators used to validate the membership of a value. It test for membership in a sequence, such as strings, lists, or tuples.

**in operator :** *The ‘in’ operator is used to check if a value exists in a sequence or not. Evaluates to true if it finds a variable in the specified sequence and false otherwise.*

**‘not in’ operator:** *Evaluates to true if it does not finds a variable in the specified sequence and false otherwise.*

#### What does the + operator mean when used with strings in Python?

It means to explicitly concatenate the strings

*fe: "spam" + "eggs"
    spameggs*

#### Explain f strings in Python?

[source](https://realpython.com/python-f-strings/)
[source](https://www.geeksforgeeks.org/formatted-string-literals-f-strings-python/)

Also called “formatted string literals,” f-strings are string literals that have an f at the beginning and curly braces containing expressions that will be replaced with their values.
*fe:*

```Python
answer = 456
f"Your answer is "{answer}""
```

#### Name 4 iterable types in Python!

1. list
2. strings
3. tuple
4. dictonory

#### What is the difference between list/set/dictionary comprehension and a generator expression in Python?

[source](https://www.geeksforgeeks.org/python-list-comprehensions-vs-generator-expressions/)

**List Comprehension:**  *It is an elegant way of defining and creating a list. List Comprehension allows us to create a list using for loop with lesser code. What normally takes 3-4 lines of code, can be compressed into just a single line.*

```python
  values = [ expression
             for value in collection
             <if condition> ]
```

```python
  a_dict = {key: value  for key, value in zip(list1, list2) if clause}
```

**Generator Expressions:** *similar to list comprehensions, but instead of creating a list and keeping the whole sequence in the memory, the generator generates the next element in demand and allows us to create a generator without the yield keyword.*

```Python
genexpr = ('Hello' for i in range(3))
```

**List Comprehension vs Generator Expressions:**

*List comprehension returns a list []
Generator expression returns an object that can be iterated through ()*

*The generator yields one item at a time and generates item only when in demand.
Whereas, in a list comprehension, Python reserves memory for the whole list.
 Thus we can say that the generator expressions are memory efficient than the lists.*

#### Does the order of the function definitions matter in Python? Why?

*It won't change the result of the program. It can help the understanding of a code if it's ordered well.
The calling of the functions is what matters.*

#### What does unpacking mean in Python?

*Unpacking in Python refers to an operation that consists of assigning an iterable of values to a tuple (or list ) of variables in a single assignment statement. As a complement, the term packing can be used when we collect several values in a single variable using the iterable unpacking operator.*

*For an example if we want to give a list as parameters of a function we can unpack the list with the "*" operator to give parameters by elements.

```Python
def fun(a,b,c,d):
    print(a,b,c,d)
my list=[1,2,3,4]
fun(*my_list)
```

#### What happens when you try to assign the result of a function which has no return statement to a variable in Python?

*If there is no return statement (or just a return without an argument), an implicit return None is added to the end of a function.*

## Software engineering

### Debugging

#### What techniques can you use while debugging a program in Python?

1. *print*
2. *debugger*
3. *rubberduck*

#### What does step over, step into and step out mean while using the debugger?

1. **step  over:**  *skip functions*
2. **step into:** *by default the debugger skips over managed properties and fields, but the Step Into Specific command allows you to override this behavior.*
3. **step out:** *to step out the specific*

#### How can you start to debug a program from a certain line using the debugger?

1. *Create breakpoint on desired line*
2. *Run to cursor(Shift + F5)*

### Version control

#### What are the advantages of using a version control system?

[source](https://www.git-tower.com/learn/git/ebook/en/command-line/basics/why-use-version-control)

1. *Collaboration*
2. *Storing Versions (Properly)*
3. *Restoring Previous Versions*
4. *Understanding What Happened (commits)*
5. *Backup*

#### What is the difference between the working directory, the staging area and the repository in git?

[source](http://archaeogeek.github.io/foss4gukdontbeafraid/git/stages.html)
[source](https://medium.com/@lucasmaurer/git-gud-the-working-tree-staging-area-and-local-repo-a1f0f4822018)
![pic](https://neurathsboat.blog/post/git-intro/featured.png)

#### What are remote repositories in git?

[source](https://www.git-tower.com/learn/git/ebook/en/command-line/remote-repositories/introduction)

Remote repos only comes into play, when when it comes to sharing data with your teammates. Think of it like a "file server" that you use to exchange data with your colleagues.

#### Why does a merge conflict occur?

*A conflict arises when two separate branches have made edits to the same line in a file, or when a file has been deleted in one branch but edited in the other.*

#### Through what series of commands could you put a new file into a remote repository connected to your existing local repository?

1. *mv - move file to that repo*
2. *git add - add to repo*
3. *git commit*
4. *git push*

#### What does it mean atomic commits and descriptive commit messages?

Atomic commits, in short, are what they sound like: atomic. I feel like there’s basically three features a commit needs to have to be atomic:

1. *Every commit pertains to one fix or feature*
2. *Don't break the build on any commit*
3. *purpose is clear from commit msges and description (descriptive commit messages)*

#### What’s the difference between git and GitHub?

Git is a distributed **version control tool** that can manage a development project's source code history, while GitHub is a **cloud based platform** built around the Git tool.

## Software design

### Clean code

#### What does clean code mean?

[source](https://learn.code.cool/full-stack/#/../pages/general/clean-code)
[source](https://gist.github.com/wojteklu/73c6914cc446146b8b533c0988cf8d29)

Code is clean if it can be understood easily – by everyone on the team. Clean code can be read and enhanced by a developer other than its original author. With understandability comes readability, changeability, extensibility and maintainability.

#### What steps do we usually do during a clean code refactoring?

1. *Bad naming*
2. *Badly formatted code*
3. *Repeated code*
4. *Long method*
5. *Wrong comment usage*
6. *Dead code*

### Error handling

#### What is exception handling?

An exception is an error that happens during execution of a program. When that
error occurs, Python generate an exception that can be handled, which avoids your
program to crash.

#### What are the basics of exception handling in Python?

[source](https://www.pythonforbeginners.com/error-handling/exception-handling-in-python)

The error handling is done through the use of exceptions that are caught in try
blocks and handled in except blocks. If an error is encountered, a try block
code execution is stopped and transferred down to the except block.

In addition to using an except block after the try block, you can also use the
finally block.

The code in the finally block will be executed regardless of whether an exception
occurs.

#### In which case should we catch an exception? Why?

Exceptions are convenient in many ways for handling errors and special conditions
in a program. When you think that you have a code which can produce an error then
you can use exception handling.

#### What can/should we do with an exception in the ‘except’ block?

1. *printing the problem in an elgegant way*
2. *quit the program if need it*

#### What does the else and finally statement do in a try-except block in Python?

**else block:** *Will be executed only if the code inside the try block doesn’t generate an exception.*

**finally block:** *Code is always executed, whether the program executed properly or it raised an exception.*

## Software Development Methodologies

#### What is the main goal of a retrospective meeting?

The goal of the retrospective is for the team members to discuss among themselves about
how the work went during the last sprint so that better ways can be found to meet the project's goals.

## Programming environment

### Unix

#### What is UNIX and what is Linux?

*Both of them are operating systems, but UNIX was earlier, it is running in CLI(Command Line Interface, meaning there is "only a command line, no mouse or graphical elements, at all)
Linux is one or more steps forward, it enables applications and the users to access the devices on the computer to perform some specific function.*

Usage:

**Unix:** *The UNIX can be used in internet servers, workstations, and PCs.*
**Linux:** *Everyone. From home users to developers and computer enthusiasts alike. Linux OS can be installed on various types of devices like mobile, tablet computers.*

#### What do we call the shell in Linux?

The shell is the **command interpreter** in an operating system such as Unix or GNU/Linux, it is a program that executes other programs. It provides a computer user an interface to the Unix/GNU Linux system so that the user can run different commands or utilities/tools with some input data.

#### What does root means in a Linux environment?

*"root" is the user name or account that by default has access to all commands and files on a Linux or other Unix-like operating system. It is also referred to as the **root account, root user and the superuser**. Basically the "System Administrator" of Linux, from Windows.*

#### How do you access your personal files in Linux?

"cd home/\<username>" in terminal 

#### How can you install an application in Linux?

*You can use Linux package managers' commands, to install an application in the terminal.
Alternative would be snap. Cannonical's own software database.*

Installing with APT:
apt install \<name_of_application>
(optional "-y" switch, to install it right away, without asking if we want to install it)
Example of installing Vim Text Editor with APT:
sudo apt install vim -y

#### What is package management in Linux, what are repositories?

[source](https://www.tecmint.com/linux-package-managers/)

*There are different Linux distributions(=distros). They share the program, also known as package manager, that manages the applications users can install, update, or delete. The most well known ones are:*

1. **DPKG:** *Debian Package Management System. Installed in Debian based distros. Very basic.
2. **APT:** *A very popular, free, powerful package manager. Also installed in Debian based distros.*
3. **RPM:** *Red Hat Package Manager. Created by RedHat. Also basic.
4. **YUM:** *Open source and popular command line package manager. It's just like APT for Debian Linux systems, but in RPM.*

#### How do you navigate in the filesystem with the command line?

1. **pwd:** *find your “present working directory”*
2. **ls:** *see the files in your current directory*
3. **cd:** *change your current directory*
    1. *To navigate into the root directory, use* **cd /**
    2. *To navigate to your home directory, use* **cd** *or* **cd\~**
    3. *To navigate up one directory level, use* **cd ..**
    4. *To navigate to the previous directory (or back),* **use cd -**
  
#### What does the following commands do: mkdir, rm, cat, cp, touch?

1. **mkdir:** *Make directory*
2. **rm:** *Remove files and directories*
```rm -rf (recursive, force) file_or_dir_name```. It is useful, when you wanna remove a non-empty directory.
3. **cat:** *Concatenate files and print to stdout.*
4. **cp:** *Copy files*
5. **touch:** *Create a new file or update its timestamp.*

#### How can you look up what does a command do in Linux if you have no internet connection?

commandname -help or commandname -h
man commandname

#### What does the following commands do: head, tail, more, less?

[source](https://linuxfrombeginning.wordpress.com/2008/09/19/linux/)

1. **head:** *displays the first **ten** lines of a file, unless otherwise stated.*
2. **tail:** *display the last part of the file*
3. **more:** *to view a text file one page at a time, press spacebar to go to the next page*
4. **less:** *is much the same as more command*

#### How do you download a file from internet using the terminal?

1. **with curl:**
    1. *sudo apt install curl*
    2. *curl –O [URL]*
    3. *curl –o [filename] [URL] # save with different filename*
    4. *curl -O [URL1] -O [URL2]*
2. **with wget**
    1. *sudo apt-get install wget*
    2. *wget [URL]*
    3. *wget -O [filename] [URL]*
    4. *wget –i [filename.txt]*
    
