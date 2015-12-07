# Computation Fundamentals

This borrows heavily from the UC Berkeley ERG Toolkits.

## Learning Objectives

- Perform simple and complex unit conversions
- Learn common energy units


## Physical Quantities
- Our numbers are often helping us represent physical quantities
- Examples:
    - The length of a tree
    - The number of animals observed
    - The number of molecules of mercury in a fish
- A physical quantity is expressed as the product of a unit and a
  numerical factor

## Dimensions
- These physical quantities often have a dimension
- Examples:
    - Length
    - Time
    - Mass

## Units
- To quantify dimensions, we use units
- One dimension may have multiple units
- Length: inches, miles, kilometers, light-years
- Mass: grams, pounds, kilograms
- There are also systems of units like SI or English

## Measurement
- Each measurement we make is an estimation of the physical quantity

## Consequences
- NASA Mars Climate Orbiter destroyed because of newton vs pounds of
force
- A cargo flight was lost in 1999 when crew confused meters and feet


## Unit conversion factors
- These factors are equivalent to one or unity and are dimensionless
- They are not numerically equal to one in most cases.
- Units can be crossed out

## Numerical Computing Environment

- Matlab
- Scientific Python
- Julia
- Sage Math Cloud

<!-- There is a subtle difference between computer programming and numerical -->
<!-- computing. -->

## Learning Objectives

- Able to use numerical computing environment to create and narrate computations
- Able to use spreadsheets to create computations




## Written
- Explanation of unit factor with inches and centimeters


## Unit Factor

$$ 1 \textrm{inch} = 2.54 \textrm{cm} $$
Dividing, we get
$$ \frac{2.54\textrm{cm}}{\textrm{inch}} = 1 $$
Note that 2.54 does not equal one, but with the units the two physical
quantities of length are equal.


## Combinations of units
- We often combine units to express new quantities



## Performing computations

While we want to develop our intuition when we are estimating with large
numbers, performing accurate calculations is also important.  You will
be able to calculate these numbers on a hand-held calculator, in Excel,
and using scientific computing platforms like Python or Julia.

## SageMathCloud

- sign up at sage math cloud
    - here is a nested list
- create notebook
- choose julia kernel
- find my publicly shared file and fill in
- print PDF and turn in during class
- markdown vs code cells
- naming variables
- shift enter to execute
- show them LaTeX


- create account
- create project
- create file jupyter notebook
- change kernel in kernel menu to Python 3 or Julia (not python 2)
- SHIFT-ENTER to evaluate your code
- up arrow moves between cells
- download as pdf

## Performing computations

While we want to develop our intuition when we are estimating with large
numbers, performing accurate calculations is also important.  You will
be able to calculate these numbers on a hand-held calculator, in Excel,
and using scientific computing platforms like Python or Julia.

Since our calculations are often used as evidence to support an
argument, they must be easy to read and have clear methods and
assumptions.  Using a computer to preserve the details of the
calculation is often preferable to using a calculator.

## Basic computations

- Addition (+)
- Subtraction (-)
- Multiplication (*)
- Division (/)
- Exponentiation (^ or **)

To perform basic calculations with numbers, we can type numbers into the
computer and use the symbols above to perform the calculation.

In the Jupyter notebook, press shift-enter to evaluate a cell.


## Variables

To make the details of a computation more clear, we can use readable
names for our numbers and then use the names in the calculation.

    power = 100
    time = 30
    energy = power * time

This makes the intention of the calculation more clear to the reader.

## Scientific Notation

$$6 \cdot 10^3$$ is entered as ``6E3``.

## Units

Computation of physical quantities often relies on the human to define
and use a consistent set of units of measurement.  There are tools that
allow us to add physical quantities to our calculations, but they are
not as rich as I could like them to be.  One good practice is to
explicitly include the unit name in the variable name.

    power_watt = 100
    time_sec = 30
    energy_joule = power_watt * time_sec



## Units

There are also computer libraries that allow you to include units in the
definition of your variables.

- Pint python library

## Defining Functions

A custom function can be created and used.  The syntax for this often
varies but the idea is usually the same.

    m = 1
    b = 10
    f(x) = m * x + b
    f(5) => 15


For Julia:

    m = 1
    b = 10
    f(x) = m * x + b

Python has a different syntax but it is the same idea.

## Narration

- You can add text and mathematics to your document
- ``# Title`` makes bold text
- ``$$ \frac{1}{2} $$`` creates mathematics $$ \frac{1}{2} $$


## Google Docs

- be sure you have access to your new sonoma.edu drive account
- access the template file that I shared
- fill in the different values and sheets

## Pandas
- assumes mastery of single variables
- now we do vector calculations (numpy or pandas?)
- to do TMY calculation we need to take difference and plot
- then we need to add up only the positive values

## Scientific Notation
- Allows us to compactly write very large or very small numbers

## Orders of magnitude
- Powers of ten
- Place value representation
- Operating on numbers with scientific notation

## Representing large numbers
- On paper
- On a calculator
- On a computer

## A very large number
- Avogadro's Number
- $$6.02 \times 10^{23}$$
- $$10^{1}$$ = 10
- $$10^{2} = 10 \times 10$$
- $$10^{3} = 10 \times 10 \times 10$$

## A very small number
- Gravitational Constant
- $$6.67 \times 10^{-11} (m^3 kg^{-1} s^{-2})$$
- $$10^{-1} = \frac{1}{10}$$
- $$10^{-2} = \frac{1}{10 \times 10}$$
- $$10^{-3} = \frac{1}{10 \times 10 \times 10}$$

<!--
http://cshsyear10maths.global2.vic.edu.au/files/2008/08/standard-form-table.png
-->

<!-- name some common units using these prefixes -->

## Operations
- Addition
- Subtraction
- Multiplication
- Division

## Scale of energy quantities
![](../figures/ipcc_energy_primer.png)
- from IPCC Energy Primer

## Energy Units
- Joule
    - SI Unit.  One Newton-Meter.
- Kilowatt-Hour
    - Energy consumed by 1 kW load over one hour
- Calorie
    - Energy to heat one gram of water one degree Celsius
- Kilo-calorie
    - One thousand calories.  Used in food energy content.
- British Thermal Unit (BTU)
    - Energy to heat one pound of water by one degree Fahrenheit
- Quad
    - One quadrillion ($10^{15}$) BTU

## Unit Conversions
- We may wish to compare energy units that are not consistent
- Often you can look up conversions in a table
- Other times you may need to recreate the conversion


## Back of the Envelope Calculations
- Construct a model of appropriate complexity
- Gather estimates of necessary quantities
- Calculate estimate
- Evaluate for feasibility

## Variables
- single values
- math expressions with variables
- sympy creation of math expressions?
- arrays
- linspace?
- treating an array like a variable
- data frames (groups of arrays)
- first use of conditionals (only add up positives or negatives)
- fancy indexing to get positives or negatives

<!--
i need to make ipython notebooks that take students through this
-->

## Worked Exercises

## Exercise
- Estimate the yearly use of gasoline in the US
- What is our strategy?

## Exercise
- How many gallons do you consume?
- How many persons in the US?

## Problems


