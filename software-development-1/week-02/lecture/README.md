# Software Development 1 
# Lecture 2 -- Introduction to Programming

## The contents of this lab will be carried out on a Jupyter Notebook. Information on using Jupyter notebooks can be found at: https://jupyter.org/

To create our Jupyter notebooks we will use Anaconda: a free and open-source distribution of the Python. Roehampton's computers should have this installed. You can download a copy for your personal computer at:
https://www.anaconda.com/products/individual

If installing, follow the prompts from the installer. Once installed, head to the "Anaconda Navigator" shortcut. 
In the Anaconda Navigator, we will have access to Jupyter Notebooks. As you launch the application, a new window in your browser will open. This is your Jupyter Notebook. Once opened, make sure to save it somewhere you can easily access. Roehampton University provides you with a Microsoft One Drive folder. Create a folder for this class (Software Development 1) and save the Jupyter Notebook as "Lecture_1.ipynb". Each .ipynb file is one notebook, so each time you create a new notebook, a new .ipynb file will be created. 

![Alt text](img_conda2.png?raw=false "Anaconda")


Jupyter Notebooks are an interactive computing environment for Python. Jupyter is an acronym for the programming languages Julia, Python and R. A Jupyter notebook integrates code and its output into a single document that combines visualizations, narrative text, mathematical equations, and other rich media. Jupyter Notebooks are now a major part of the data science workflow. 

In this lab, we’ll explore 
1.  What is Programming (Video/ Exercises)
2.  Programming Languages (Video/ Exercises)
3.  Introduction to Python (Video/ Exercises)

By the end of this lab and its accompanying seminar, you’ll be able to run Python code via Jupyter Notebooks. You’ll have knowledge of programming concepts, programming skills and problem-solving abilities. Our goal is to make you think as a computer scientist so that when you are faced with a challenge, you’ll immediately think:

> "How am I going to write a piece of code to help me tackle this?"

A few tips: Practice, practice, practice. You can’t passively absorb programming as a skill. Please view the videos before lecture so that you can maximise our time together. Remember that your instructor is not a mind reader, please tell them when you are struggling. Finally, don’t be afraid to try your code, you won’t break your computer!

Let’s get started.
### Exercise
    # Our first Python program, print out "Hello, world"
    
    print("Hello, world")

fun fact: Brian Kernighan wrote the first "hello, world" program as part of the documentation for the BCPL programming language developed by Martin Richards. BCPL was used while C was being developed at Bell Labs a few years before the publication of Kernighan and Ritchie's C book in 1972.

## Lesson 1:  What is Programming?

Video: https://roehampton.cloud.panopto.eu/Panopto/Pages/Viewer.aspx?id=94ff6a2b-948b-4b73-adb2-ac4900c517a5

To understand this, we need to separate computer from computation. Computation is independent of the way is it is implemented in a computer. Think of the difference between knowing something vs knowing how to do something. For instance, knowing what is your favourite food vs how to make your favourite food. 

    Exercise: Do you know how to make you favourite food? Can you write down a recipe for how to make it?

A recipe is a description of a set of steps; a sequence of specific instructions in order for you to accomplish an objective. 
We define computation as the techniques of capturing this process in a mechanical fashion.

Some of the earliest computers, known as **fixed program computers**, were designed to do just one thing. For instance, early calculators were designed to do only maths. In the 1940’s Dr Alan Turing made the Bombe computer with the sole purpose of breaking German code (cryptography). Trough computing, we want to capture the idea of problem solving.

 > Suppose you invent a circuit that reads a circuit diagram and reconfigures itself to act like that that circuit diagram. You would have to invent a machine that takes a recipe, and acts like what is described in that recipe. This is known as an interpreter. 
     What happens when you change the circuit?

This is the idea behind **Stored Program Computers**, the multipurpose device we will be working with. These computers usually have the following elements:

    Memory-> Control Unit-> ALU-> Programme Counter
    
![Alt text](img_stored_program.png?raw=false "Stored Program Computer")

Programming is the process of creating a set of instructions that tell a computer how to perform a task. Programming can be done using a variety of computer programming languages, such as Matlab, Python, and C++

Back in the olden days, computers had physical cards that need punching, etc. 

    Do you know of any of these old physical computing mechanisms? 
    
    
### Exercises
Let's use Python as a Fixed Program Computer such as a Calculator

    1. How many seconds are there in 42 minutes 42 seconds?
    
    2. How many miles are there in 10 kilometres? 
    Hint: there are 1.61 kilometres in a mile.
    
    3. If you run a 10 kilometres race in 42 minutes 42 seconds, 
    what is your average pace (time per mile in minutes and seconds)? 
    What is your average speed in miles per hour?
    

## Lesson 2: Programming Languages

Video: https://roehampton.cloud.panopto.eu/Panopto/Pages/Viewer.aspx?id=92cb69a2-0d52-4b23-ae58-ac4900c51714

To describe recipes, we need a language. So far, we have been using English to describe these recipes. However, to be able to communicate with the computer, we need a different language. Our digital devices understand instructions in 1s and 0s. The basic programming languages take this into account and create basic words or instructions that translate into something the computer can do with those 1s and 0s. We discussed how some of these old computers had tapes and other mechanical mechanisms to handle instructions and data. The first computer languages then needed to translate our commands to something the computer could understand. From these a basic set of instructions, or primitives, were born.

> Given a fixed set of primitives (defined then as the most basic instructions for the Stored Program Computers to work) we can program anything. 

1936 Turing showed that with 6 primitives (having to do with the way tapes are being read or written), anything that can be described in a mechanical process, can be programmed with those 6 primitives. Furthermore, he showed that anything that you can do in one programming language you can do in another programming language (Turing compatibility). Fast forward 90 years, the languages have gotten more complex with many more higher-level primitives that more closely resemble our human languages. Square root can be a primitive.

We’ll explore some of these modern primitives, how we make them and understand how the affect the flow of control. Like human languages, there are 100s of programming languages including Visual Basic, C, Mathematica, Matlab, C++, Java, Processing and Python. 

We’ll use **python** for this class, but this course is not about **python**. We need to know how to use it, but it’s not about where do the semicolons go in Python. It’s about using Python as a tool to think. We are interested here in learning how to learn, how to design recipe, how to structure recipes, how to do things in ways that can be translated to other languages. Once you know how to think like this, you can then learn another language in a few weeks.

We refer to the *“dimension of language”* when we are asking how close are we to the guts of the machine?
> *Assembly language* is when you are programming at the level of the primitives, moving one piece of data from one location in memory to the next. 
> *High level language* is a more recognisable set of actions. For example, when you ask Python to *print* some information, it will literally print in the display the information. 


When we discuss *General* vs *Targeted* languages, what we want to know is how broad are the applications. Are they very specific or can they be used for many things?
> Matlab, for instance, is a language targeted to Matrices.


Finally, when we ask whether a language is *Interpreted* vs *Compiled*, we are asking whether the source code goes directly to an interpreter, or if the source code first runs into a checker or compiler and then creates object code. The latter helps catch bugs in the code and converts it into a more efficient sequence of instructions that you then run. It’s not as fast as going directly to the interpreter though. 

> Therefore, Python is a high level, general purpose, interpreted language.

### Exercises
Let's use Python to form a recipe to calculate for the following:

    4. The volume of a sphere with radius r is 4/3 π r^3 . 
    What is the volume of a sphere with radius 5? 
    How about radius 3.5? 
    
    5. Suppose the cover price of a book is $24.95, but bookstores get a 40% discount. 
    Shipping costs $3 in the US for the first copy and 75 cents for each additional copy.
    What is the total wholesale cost for 40 and 60 copies in the US? 
    In the UK shipping costs £4.50 and £1.90 for each additional copy.
    Today, 1 US dollar = 0.77 British pounds.
    What's the total for 40 and 60 copies in the UK? 
    
    6. I leave my house at 6:52am. I run:
       1 mile at an easy pace (8:15 per mile) 
       3 miles at tempo (7:12 per mile) 
       1 mile at an easy pace again. 
       At what time do I get home for breakfast?
    

## Lesson 3:  Introduction to Python

Video: https://roehampton.cloud.panopto.eu/Panopto/Pages/Viewer.aspx?id=058f6deb-ebd6-4f9f-90eb-ac4900c51768

Python Syntax vs Semantics
> Syntax says what are the legal expressions in this language (cat, dog, etc)
> Semantics says how we construct expressions

*Static Semantics* in Python determine which programs are meaningful; which expressions make sense. Consider for instance: 
    My desk is Susan

Does it make sense?

    False.

*Static Semantics* asks what does the program mean? What’s going to happen when I run it? Thought this, Python checks your syntax, one bug at a time.

Typical Problems that can arise are: 
    It could not run, it could loop forever, or it gives you a wrong answer. 

But the problem is that if the program is complex enough you might not be able to tell! To help tackle this, we need to develop a **good style**: write in a way that allows you to spot problems.

The goal for this lab session is to have a set of primitives that we combine into complex expressions that we can then abstract and treat as *higher primitives*. For this, we will use a sequence of instructions in this flow of control in order to deduce new information. 


Python has different Types of values: 

> Strings are **strings**

> Numbers can be **integer, floats**

> Logical (true or false) are **Boolean**

Higher programming languages have a set of operators that expect a certain type of input to give a certain type of output. Let’s explore the typical set of arithmetic operations:
>    5*5

>    3+2

>    7/3


What do these have in common?

    Operand operator operand

What happens if we do something like “cat”/“tree"?

    Error

Commands (statements) take a value and ask the computer to do something with it. 

    What is the difference between:
    
    print (5*4)
    
    print (“5*4"")
    
    print (“5”*"4”")


Finally, we use Variables to store things

    mystringis = (assign or bind to this name the value of this expression)
    
We’ll continue exploring variables in the next session.
    

## Style Tips
### Naming
Variables, functions, methods, packages, modules

*lower_case_with_underscores*

### Exercises
We'll explore and expand on some of these concepts in Python via your open Jupyter Notebook. 


    7.What does the variable counter contain after the following code runs? 

    counter = 20
    counter += 1 
    counter
    
    8. Identify what kind of values each one is with type()
       3 * 4
       ‘hi’ 
       -99.1
       False
       4 - 6.0
       3.0 / 6
       0 + 0
       "2.0"
       0.00
       2**3
       “My dog ate my homework"
       7 == 3 + 4
    
    9. Search online for the Python documentation for the len() function. 
    It will be on a web page titled “Built-in Functions.” 
    Skim the list of other functions Python has. 
    Look up what the round() function does, and experiment with it.


FIN 
