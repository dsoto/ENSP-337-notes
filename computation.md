# Introduction

While we want to develop our intuition when we are estimating with large
numbers, performing accurate calculations is also important.  You will
be able to calculate these numbers on a hand-held calculator, in Excel,
and using scientific computing platforms like Python.

Since our calculations are often used as evidence to support an
argument, they must be easy to read and have clear methods and
assumptions.  Using a computer to preserve the details of the
calculation is often preferable to using a calculator.

We will start with concepts most familiar to you from your work with
calculators and we will build more concepts on that knowledge.

# Basic Concepts

- Computing platforms
- Computing languages
- Arithmetic operations
- Variables
- Functions

## Computing platforms

- You are likely most familiar with a calculator
- You enter a series of commands
- When you press enter or equals, they are sent to a small computer for
    evaluation
- The results are printed for you
- There are many computer programs that do similar things and allow much
    more power and flexibility
- Other platforms are Mathematica and spreadsheets

## Basic computations

- Addition (+)
- Subtraction (-)
- Multiplication (*)
- Division (/)
- Exponentiation (^ or **)

To perform basic calculations with numbers, we can type numbers into the
computer and use the symbols above to perform the calculation.

## Computing languages

- Computing languages allow us to instruct the computer to do things
- As our models and computations become more complex, we will want to do
    things besides addition and multiplication
- Using a computing language helps us achieve that

## Variables

To make the details of a computation more clear, we can use readable
names for our numbers and then use the names in the calculation.

```
power = 100
time = 30
energy = power * time
```

- This makes the intention of the calculation more clear to the reader.
- This also allows us to reuse what we have typed and change our numbers
    easily to repeat a similar calculation

## Functions

You have often used functions on your calculator and you have
encountered the idea in your math classes.

A function takes a number or numbers as an input and provides a number
or numbers as an output.

You have probably used sine or cosine functions on your calculator.

You may want to make your own function for a calculation that you do
frequently.  The syntax for this often varies but the idea is usually
the same.

```
m = 1
b = 10
f(x) = m * x + b
f(5) => 15
```

## Print Function

Computer functions can take many things besides numbers as input and do
many things besides return numbers as output.  The print function is
very useful.  Provided with text or variables, it will output things to
the screen.

```
estimate = 20
print('My estimate: ', estimate)

> My estimate: 20
```

# Jupyter Concepts

- Markup and Markdown
- Markup and LaTeX
- Python
- Jupyter

## Jupyter

- Jupyter is like a word processor and spreadsheet in one program
- By mixing words and computations together, you can clearly explain
    your approach to an estimation
- It has blocks or cells of text that are sent to the program of your
    choice to be interpreted
- Markdown: our word processor
- Python: our spreadsheet or computation program
- You press shift-enter to evaluate a cell

## Markdown

- You can think of this as a word processor
- By selecting markdown as the type of cell, jupyter sends the text to
    markdown to be interpreted
- Special characters are use to tell the computer to make headings or
    bold characters

## LaTeX

- This is a word processor especially for math
- By placing dollar signs ($) around some text, it is sent to LaTeX to
    be interpreted
- You can use this to write fractions and many other mathematical
    symbols
- You can find some symbols at this
    [link](http://estudijas.lu.lv/pluginfile.php/14809/mod_page/content/16/instrukcijas/matematika_moodle/LaTeX_Symbols.pdf)

For example

```
\frac{1}{2}
```

will turn into

$$\frac{1}{2}$$


## SageMathCloud

We use SageMathCloud to provide an easy-to-use platform for our
computations

- Create an account at Sage Math Cloud
- Use your nice_person@sonoma.edu email address

- We will add you to our class
- You will be able to access class content and various tools

