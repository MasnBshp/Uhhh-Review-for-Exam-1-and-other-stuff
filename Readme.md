## A Semi-Decent Review of the Python Book we use as well as tips and random stuff.

   
    What a Program is:  The definition of a program at its most basic is a sequence of Python statements
    that have been crafted to do something. Even our simple hello.py SCRIPT is a
    program. It is a one-line program and is not particularly useful, but in the strictest
    definition, it is a Python program.


                    Definitions and Common language you'll hear

    INPUT:   Get data from the “outside world”. This might be reading data from a
    file, or even some kind of sensor like a microphone or GPS. In our initial
    programs, our input will come from the user typing data on the keyboard.        Indentified by Input()

    OUTPUT:  Display the results of the program on a screen or store them in a file or
    perhaps write them to a device like a speaker to play music or speak text.      Indentified by whatever is printed out by the computer when the script is ran

    CENTRAL PROCESSING UNIT:     The heart of any computer. It is what runs the software
    that we write; also called “CPU” or “the processor”.

    PROMPT:     When a program displays a message and pauses for the user to type some
                input to the program.
                
    BUG:    An error in a program.

    SEMANTIC ERROR:  An error in a program that makes it do something other than
    what the programmer intended.

    SEQUENTIAL EXECUTION:    Perform statements one after another in the order they
    are encountered in the script.

    REPEATED EXECUTION:    Perform some set of statements repeatedly, usually with
    some variation


    TYPE:       A category of values. The types we have seen so far are integers (type int),
                floating-point numbers (type float), and strings (type str).

    VALUE:      One of the basic units of data, like a number or string, that a program manipulates.    
    
    VARIABLE:   A name that refers to a value

    STATEMENT:  A statement is a unit of code that the Python interpreter can execute.      An line of code is theoritically a statement, this whole review is one in some way

    SCRIPT:     A script usually contains a sequence of statements.

    STRING:     A type that represents sequences of characters.    Ex. "Pineapple does not belong on Pizza", "Hello World!"       Indentified by Str()

    INTEGER:    A value or variable that represents a whole number.   Ex. 2, 3, 99, 7298342       Indentified by Int()

    FLOAT:      A value or variable that represents a decimal number, also known as floating point  Ex. 2.5, 3.1, 99.9, 7.298342        Indentified by Float()

    BOOLEAN:    A boolean expression is an expression that is either true or false.    Ex. 5 == 5 ---> The output is True 5 == 6 ---> The output is False       Indentified by bool()

    MODULUS:    An operator that works on integers and yields the remainder when one number is divided by another.     Ex. 3 % 2 = 1, 6 % 4 = 2     Indentified by %

    EXPONENTATION:     An operator that raises the power of a value by itself, "to the power of".       Ex. 3**2 = 9, regular math its 3^2       Indentified by **

    FLOOR DIVISION:    An operator that divides two integers and rounds down to the nearest whole number, also known as integer division.   Ex. 15 // 2 ---> The output is  7      Indentified by //

                      
                I don't believe I need to explain how addition, subtraction, division, etc. works so I'll just show their respective operator.
    
    + is Addition          * is Multiplication      % is Modulus                                // is Floor Division
    - is Subtraction       / is division            ** is Exponent or to the Power of           
            


    COMMENT:    A "#" is used to turn the line into an unreadable part when you run the program, (place it at the front)

    EXPRESSION: An expression is a combination of values, variables, and operators. A value all by
    itself is considered an expression, and so is a variable

    PEMDAS:  For the way Python follows a statement. When more than one operator appears in an expression, the order of evaluation
    depends on the rules of precedence. For mathematical operators, Python follows
    mathematical convention. The acronym PEMDAS is a useful way to remember
    the rules.

    OPERATOR:  A special symbol that represents a simple computation like addition,
    multiplication, or string concatenation.    Ex. +, -, !=, >, etc.

    OPERAND:   One of the values on which an operator operates.     Ex. 3 + 10      a = 30, b = 20 ("a" and "b" are operands)
                                                                        ^    ^  ("3" and "10" are operands while the "+" is an operator)

        The == operator is one of the comparison operators; the others are:

              Statement:           Reasoning:

                x != y          x is not equal to y
                x > y           x is greater than y
                x < y           x is less than y
                x >= y          x is greater than or equal to y
                x <= y          x is less than or equal to y
                x is y          x is the same as y
                x is not y      x is not the same as y





    SEQUENTIAL EXECUTION:    Perform statements one after another in the order they
    are encountered in the script.

    CONDITIONAL EXECUTION:   Check for certain conditions and then execute or skip a
    sequence of statements.

    REPEATED EXECUTION:  Perform some set of statements repeatedly, usually with
    some variation.

    REUSE:   Write a set of instructions once and give them a name and then reuse those
    instructions as needed throughout your program.

    IMPORT STATEMENT:    A statement that reads a module file and creates a module object.

    MODULE OBJECT:   A value created by an import statement that provides access to the data and code defined in a module.


                Python reserves 35 keywords:

    and         del         from        None            True
    as          elif        global      nonlocal        try
    assert      else        if          not             while
    break       except      import      or              with
    class       False       in          pass            yield
    continue    finally     is          raise           async
    def         for         lambda      return          await


            This section is just based on imports, inputs, and types or changes

        
    input() allows the user to type a value with their keyboard.    
        Ex. user_option = input("What is the menu option you want?") or name = input("What is your name")
            whatever = input()           print(whatever) ---> whatever was inputed by the user

    


    int() changes the user's input into an integer.    
        Ex. prompt = 'What...is the airspeed velocity of an unladen swallow?\n' 
            speed = input(prompt)
            What is the airspeed velocity of an unladen swallow?
            17
            int(speed)
            17
            int(speed) + 5
            22


    str() changes the value to a string.
        Ex. week = 33                                           number = 999                                    str(123)
            greeting = "it is week " + str(week)                number_as_string = str(number)                  '123'
            greeting                                            number_as_string
            'it is week 33'                                     '999'

    float() chnages the value to a float.
        Ex. time1 = 4
            time2 = 3
            final_time = float(time1 + time2)

    IMPORT FUNCTION:    The best way I'd describe the "import" function is bringing in a function or program into your code. We've used them for the dice game, import random, to
    allow the code to choice a random number from 1-6 for the dice roll. There are other ones like: import math, import "othercode.txt" (so we can use another code), as well as
    import certain parts from programs by doing: Ex. from math import addition

    Alternative Execution: A second form of the if statement is alternative execution, in which there are two
    possibilities and the condition determines which one gets executed. The syntax
    looks like this
        if x % 2 == 0 :
            print('x is even')
        else :
            print('x is odd')



                                        Executions and most recent topic

    Condtional Execution: In order to write useful programs, we almost always need the ability to check conditions and change the behavior of the program accordingly. Conditional statements
    give us this ability.

        if x > 0 :
        print('x is positive')
    
    Sometimes there are more than two possibilities and we need more than two
    branches. One way to express a computation like that is a chained conditional:

        if x < y:
            print('x is less than y')
        elif x > y:
            print('x is greater than y')
        else:
            print('x and y are equal')
            
    Nested Conditionals: One conditional can also be nested within another. We could have written the
    three-branch example like this:

        if x == y:
            print('x and y are equal')
        else:
        if x < y:
            print('x is less than y')
        else:
            print('x is greater than y')
            


                                                Tips and shortcuts you should utilize:

ctrl + s    is to save file
ctrl + c    is to copy text
ctrl + z    is to undo action
ctrl + b    is to hide or unhide the EXPLORER tab on the left side
ctrl + n    is to create a new file
ctrl + /    turns the lines highlighted into comments
ctrl + [ or ] allows you to add or remove indents
ctrl + Home/End allows you to go to the beginning or end of the line
ctrl + f    opens the find menu
ctrl + enter goes to next line

And go to the Help tab on the top left so you can see more keybinds as well as create your own keybinds
