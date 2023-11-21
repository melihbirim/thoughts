# Why Programming Is Really Hard To Learn?

## Abstract:

This paper introduces a simplified programming language designed for ease of learning, especially for beginners. 

With just 6 keywords and a structure mirroring natural human language, it aims to make programming more intuitive and accessible. 

The effectiveness of this language is demonstrated through a Fibonacci sequence example, highlighting its potential to simplify complex programming concepts. 

This approach seeks to bridge the gap between human communication and computer logic, making programming an approachable skill for a broader audience.

## Introduction
Have you ever thought about how computers work? They use a special language made up of 0s and 1s. But for us humans, this language is really hard to understand. 

That's why we have programming languages – they help us talk to computers in a way that's easier for us to understand. 

But even these languages can be tricky. They have lots of rules and words that you need to remember, which can be overwhelming, especially if you're just *starting to learn*.

In this article, I've come up with a new way to make programming simpler. Imagine a language that's as easy as talking to a friend. That's what I'm trying to do. My language has just a few keywords, six, and it's designed to make programming feel more natural and less confusing.

To show you how it works, I used this language to write a program for something called the Fibonacci sequence. It's a series of numbers where each number is the sum of the two before it. This example shows that even with a simple language, you can do cool things.

So, if you've ever felt like programming is too hard, or if you're curious about how to talk to computers, this article is for you. I want to show you that programming can be easy and fun, just like having a chat. Let's dive in and see how we can make computers understand us better!

## The Language

In this section, I'll introduce the core concept of the simplified programming language I've designed or I would say thought. Till now, there is not any defined grammer, it is just a concept. The primary goal is to make programming more accessible by reducing complexity and mimicking natural human language patterns. 

And I would like to call the language `1im`.

### Overview
The language should be on a foundation of simplicity and intuitiveness. It uses only six keywords, at max, to avoid the need of memorizing dozens of commands and understanding complex syntax or indetation rules. 

This minimalist approach is designed to lower the barrier to *entry* for programming, making it more *approachable* for beginners, especially for kids and those intimidated by the typical learning curve of standard programming languages.

### Key Features

#### Simplicity in Syntax: 
The syntax of the language is straightforward and easy to understand. It avoids complex structures, focusing instead on clear, concise commands that reflect everyday language. 

#### Limited Keywords: 
With only a handful of keywords (def, if, else, set, loop, and end), the language reduces the cognitive load on the learner. Each keyword has a specific, easily understandable purpose, aligning closely with its natural language counterpart, -- may be I can add 'begin' as another keyword. I decided to continue on indentation as a first citizen to remove other keywords

#### Natural Language Flow: 
The structure of the language encourages a flow that resembles how we speak or write in everyday situations. This natural flow makes it easier for beginners to translate their thoughts into code also using math syntax they have learned in primary schools.

#### Flexibility and Power: 
Despite its simplicity, the language is designed to be powerful enough to handle a range of programming tasks. The Fibonacci sequence example illustrates how even with limited keywords, the language can effectively implement complex algorithms.

### Language Definition
#### Syntax

*Keywords:* The language has a limited set of keywords which is 6: ```if, else, set, to, with, loop```.
*Structure:*
with number1, number2, number3
- Functions: ```set ${functionName} with ${[input parameters]} ...{indented } ```
- Conditional: ```if [condition] ... [else | else if] ... end```
- Variable Assignment: ```set [variable] [value]``` or ```set [variable] to [value]```
- Loop: ```loop [condition] ...```


*Expressions:*
*Arithmetic:* Supports basic arithmetic operations (+, -, *, /)

*Logical:* Incorporates simple logical operations (>, <, ==, !=)

Parentheses for precedence: (expression)

*Comments:* Single line comments start with #.

#### Semantics

Variables: 
- Dynamically typed, where the type is inferred from the assigned value.

Control Structures: 
- `if` and `else` for conditional execution.
- `loop` for iteration, which continues as long as the condition holds true.
 
Function Definition and Invocation:
- Functions are defined with `set` and `with` keyword for input argument.
- Parameters are passed by value.
- It has implicit returns, it can retun as many variable as possible, the only constraint is to have it as the last line. This can avoid the use of another keyword. e.g ruby. elixr

#### Core Functionalities
- Variable Assignment and Management: The set keyword is used for declaring and assigning values to variables and functions.
- Conditional Logic: if and else are used for decision-making processes.
- Loops: The loop keyword facilitates iterations.
- Functionality Scope: Each function and loop has its own scope.

#### Error Handling
Basic error handling includes syntax errors, type errors, and runtime exceptions.
Error messages are designed to be understandable and helpful.

#### Example Implementation

Fibonacci sequence using the language:
```lua
set i to 1, p to 1, total to 0
set count to 100
loop if count < limit
  set total to (i + p), count to (count + 1)
  set i to p, p to total
end

# functions
set addNumbers with number1, number2
  set sum to (number1 + number2)
  sum # This is the implicit return value

set sum to addNumbers 1,2
```

