# Programming Basics questions

## Computer science

### Data structures

#### What is the purpose of a list (array in some programming languages) data structure? Name some methods of it!

*The purpose of a list/array, is to store different variables, close to each other. Like names.*

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

![pic](https://res.cloudinary.com/practicaldev/image/fetch/s--s1Qbl8Gf--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/mwcwre09s12vqa3gvl7a.png)

#### What is “Stack overflow”?

**An error type.**
*In softwarem a stack overflow occurs if the call stack pointer exceeds the stack bound. The call stack may consist of a limited amount of address space, oftendetermined at the start of the program. The size of the call stack depends on many factors, including the programming language, machine architecture, multi-threading, and amount of available memory. When a program attempts to use more space than is available on the call stack , the stack is said to overflow, typically resulting in a program crash. Recursive function never quit.*

#### What are the main parts of a function?

```Python
def random(arg1, arg2): # function signature(function name,paramater list)
    multiply = arg1+ arg2 # function body
    return multiply
```

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
