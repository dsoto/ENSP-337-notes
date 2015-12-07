# Lecture 01

## ENSP 337, Lecture 1, Introduction and Overview
**Professor Daniel Soto, Sonoma State University**

**26 Aug 2015**


<!-- 50 min syllabus and introduction -->
<!-- 50 min group activity and discussion -->
<!-- how many read Cal Newport or Barbara Oakley books? -->
<!-- how many students overlap in both classes? -->


## Your learning goals

- Form groups of two or three and discuss the following
- Why are you taking this class?
- What are your learning goals for this class?

<!-- skills vs credential -->


## Learning Objectives

- Understand how this class will function
- Understand the larger context for thermal energy



## Instructor Expectations

- I will be on time and prepared for every class
- I will give assignments that develop your skills
- I will respect students
- I will make my grading guidelines clear
- I will respond to email within 48 working hours


## Student Expectations

- I expect you attend class consistently
- I expect you to respect your classmates
- I expect you to give your full focus during class
- I expect you to fully participate in class activities


## Syllabus
- The syllabus has a link on Moodle
- The syllabus changes during every semester
- I will announce any updates to the syllabus


## Existing knowledge
- What do you already know about thermal energy?


<!-- What thermal services are delivered in your daily life? -->
<!-- How do you cook food in your home? -->
<!-- How do you heat water in your home? -->
<!-- How is your home heated? -->
<!-- How is the ETC building heated? -->
<!-- How are you heated? -->
<!-- How is your home cooled? -->
<!-- How is your food cooled? -->
<!-- What energy transformations take place in all these? -->


## Interviews
- What do you want to learn in this class?
- What skills do you want to develop?
- Why do you think these skills are important?


# Lecture 02


## ENSP 337, Lecture 2, Introduction and Overview

**Professor Daniel Soto, Sonoma State University**

**31 Aug 2015**


## Learning Objectives

- Recognize key thermal energy concepts
- Recognize how thermal energy use fits in global energy system

<!-- TODO: find citation for half of US primary energy in buildings -->

<!-- orient global thermal energy context -->
<!-- heat is intermediate for all energy -->
<!-- equilibrium temperature bathtub model -->
<!-- concepts of temperature -->



## Thermal energy concepts

- Temperature
- Internal energy
- Heat (transfer)
- Heat capacity
- Conduction
- Convection
- Radiation
- Combustion

## Energy conversion and efficiency

- What primary energy sources do we use for heat?
- How efficiently do we capture and move thermal energy?


## Energy terms

- End use: what the energy is used for at the instant of consumption
- Primary energy: what is the original consumption in terms of
    energy


## US Commercial Building End Use
![US Commercial Building End Use](../figures/commercial-end-use-DOE.png)


## US Residential Building End Use
![US Residential End Use](../figures/residential-end-use-DOE.png)


## US Buildings
![Buildings use more primary energy than all of Russia](../figures/RMI-building-energy.jpg)


## Activity

What do you already know about each of these thermal energy concepts?


## Activity

- What questions do you want to answer in this class?

## Estimation Activity

- How much air conditioning energy is used by American homes this year?


## Activity

- What phenomena cause some observable things in our lives?

## Demonstrations

- Calca
- Sage Math Cloud

## Bathtub model

- Energy
- Appliances
- Building Stock





# Lecture 03

## ENSP 337, Lecture 3, Units and Conversions

**Professor Daniel Soto, Sonoma State University**

**02 Sep 2015**


## Learning Objectives

- Perform simple and complex unit conversions
- Learn common energy units


## Required purchase?

- Sage Math Cloud would cost $15 per student

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


## Energy vs Power

- Power is the rate of energy transfer or delivery
- Average power is the amount of energy transferred or converted divided
  by the time spent


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
- Therm
    - 100,000 BTU


## Energy Unit Table

| Unit          |             | Joule Equivalent |
| ----          | -----       | -----            |
| Joule         |             |                  |
| Kilowatt-Hour |             | 3.6 MJ           |
| BTU           |             | 1055 J           |
| Calorie       |             | 4.186 J          |
| Food Calorie  |             | 4186 J           |
| Therm         | 100,000 BTU |                  |


## Power Units

- Watt
    - One joule converted in one second
- Horsepower
- BTU/hour (sometimes just called BTU)


## Power Unit Table

| Unit       |       | Watt Equivalent |
| ----       | ----- | -----           |
| Watt       |       |                 |
| BTU/hour   |       | 0.293 Watt      |
| Horsepower |       | 750 Watt        |


## Activity

- Show that one kilowatt-hour is equal to 3.6 MJ.




# Lecture 04

## ENSP 337, Lecture 4, Computational Tools/Investment

**Professor Daniel Soto, Sonoma State University**

**02 Sep 2015**

## Learning Objectives

- Able to use numerical computing environment to create and narrate computations
- Able to use spreadsheets to create computations
- We may touch on the time value of money at the end

## Numerical Computing Environment

- Matlab
- Scientific Python
- Julia
- Sage Math Cloud

<!-- There is a subtle difference between computer programming and numerical -->
<!-- computing. -->

## Sage Math Cloud

- How many folks have signed up?
- Review homework template on SMC

## Basic computations

Most mathematical software uses the following symbols for basic
arithmetic.

- Addition (+)
- Subtraction (-)
- Multiplication (*)
- Division (/)
- Exponentiation (^ or **)

To perform basic calculations with numbers, we can type numbers into the
computer and use the symbols above to perform the calculation.

In the Jupyter notebook, press shift-enter to evaluate a cell.


## Scientific Notation

$$6 \cdot 10^3$$ is entered as ``6E3``.


## Cells

We place a group of computations together in a cell.

## Variables

To make the details of a computation more clear, we can use readable
names for our numbers and then use the names in the calculation.  Most
mathematical software use this simple syntax.

    power = 100
    time = 30
    energy = power * time

This makes the intention of the calculation more clear to the reader.

## Functions

A custom function can be created and used.  The syntax for this often
varies but the idea is usually the same.

For Julia:

    m = 1
    b = 10
    f(x) = m * x + b

Python has a different syntax but it is the same idea.


## Narration

- You can add text and mathematics to your document
- ``# Title`` makes bold text
- ``$$ \frac{1}{2} $$`` creates mathematics $$ \frac{1}{2} $$


## Units

Computation of physical quantities often relies on the human to define
and use a consistent set of units of measurement.  There are tools that
allow us to add physical quantities to our calculations, but they are
not as rich as I could like them to be.  One good practice is to
explicitly include the unit name in the variable name.

    power_watt = 100
    time_sec = 30
    energy_joule = power_watt * time_sec

<!-- excel has custom formats for units? -->

## Units

There are also computer libraries that allow you to include units in the
definition of your variables.

- Pint python library

<!-- show pint examples -->

## Activity

- Create a Sage Math Cloud account
- Access the homework assignment


# Lecture 05, Time Value of Money


# Lecture 6, Time Value of Money




# Lecture 7, Energy and Power and Heat

## Learning Objectives

- Understand and calculate heat capacity to find energy needed to raise
    temperatures

## Review

- Power
- Energy
- Heat
- Units

## Heat
- Heat is the flow of this energy from one area to another
- Conduction
- Convection
- Radiation


## Intensive vs Extensive Properties

- Intensive or bulk property
    - Does not depend on the amount of material
    - Example: temperature, density
- Extensive property
    - Depends on the amount of material
    - Example: mass, volume


## Temperature
- Measure of the internal energy in a system or material
- This energy is the motion, vibration, or rotation of atoms and
  molecules


## Temperature Scales
![](../figures/temperature_scales.jpg)


## Heat Capacity

- When heat moves from one material to another one temperature rises the
    other falls
- The change in temperature is dictated by the heat capacity
- Ratio of heat added to temperature change


## Heat Capacity

- Extensive property
- Measured in Joules per degree Kelvin


## Specific Heat Capacity

- Intensive property
- Measured in Joules per mass per degree Kelvin


## Table of Specific Heat Values

| Material | Heat Capacity (Joule/gram/kelvin) |
| --       | --                                |
| Air      | 1                                 |
| Water    | 4.1813                            |
| Iron     | 0.45                              |
| Aluminum | 0.897                             |
| Brick    | 0.840                             |
| Wood     | 1.2 - 2.9                         |

Partial list from https://en.wikipedia.org/wiki/Heat_capacity


## Heat capacity

$$ Q = mc\Delta T $$

- $Q$ is energy transferred to or from substance
- $m$ is the mass
- $c$ is the specific heat capacity
- $\Delta T$ is the temperature change


## Relation to Buildings

- Thermal mass is added to a building to store heat


## Relation to Weather and Climate

- The heat capacity of water affects the climate in some areas


## Activity

- Can we estimate the power of the tea kettle?

    volume = 1 liter
    mass_water = 1000 gram
    time = 5 * 60 sec => 300 sec
    heat_capacity = 4.186 joule/gram/kelvin
    temperature_change = 75 kelvin

    mass_water * heat_capacity
    * temperature_change / time in watt => 1,046.5 watt

This is very close to our measure value of 1300 watts.


# Lecture 8, Combustion

## ENSP 337, Lecture 8, Combustion

**Professor Daniel Soto, Sonoma State University**

**23 Sep 2015**


## Learning Objectives

- Calculate carbon emissions resulting from combustion and electricity
- Calculate energy released by combustion

## Concepts

- Energy density
- Carbon emissions

## Activity

- Predict what time the kettle will reach 100C


## Prediction

    delta_T = (100K - 20.8K) => 79.2 K
    m_water = 750 gram
    c_water = 4.186 J/gram/K
    power = 1340 J/sec

    m_water * c_water
    * delta_T / power
    * => 185.5585 sec



# Lecture 9, Conduction

## ENSP 337, Lecture 9, Conduction

**Professor Daniel Soto, Sonoma State University**

**28 Sep 2015**

## Plan

- Intro 15 min
- Homework Swap 30 min
- Conduction lecture 45 min

## Learning Objectives

- Estimate the energy flow through conductive materials
- Understand linear relationships


# Lecture 10, Conduction

## ENSP 337, Lecture 10, Conduction

**Professor Daniel Soto, Sonoma State University**

**02 Sep 2015**

# Lecture 14, Midterm Review

## Midterm
- Quantitative
- Conceptual
- Letter size cheat sheet allowed and turned in
- No internet

## Topics
- Units and conversions
- Computational tools
- Time value of money
- Investment metrics
- Energy and Power and Heat
- Combustion
- Conduction
- Convection

## Concepts
- Heat Capacity
- Conductive Heat Transfer
- Time Value of Money

# Lecture 15, Midterm


# Lecture 18

## Lecture 18, Thermodynamics

## Deadlines
- Load up coolers on afternoon of Tuesday Nov. 17th

## Homework
- Temperature conversion issues
- Everyone can do 3.6 over for full credit

## Questions
- How much power does a refrigerator use?
- Could you use a refrigerator to heat and cool your house?
- What is the most mechanical work you can extract from heat energy?
- What is the most heat energy you can extract with work?

## Activity
- Estimate the average power of the refrigerator in the ETC



# Lecture 20, Monday 9 Nov 2015, Metrics

## Metrics
- How do we estimate the energy use for a home?


## Homework 3.7 and 3.8
- 3.7
    - surface area of cylinder
    - units of area
    - Square millimeters vs square meters
- 3.8
    - surface area of cube
    - units of area

## Heating Degree Days
- How much energy will it take to heat the ETC this winter?



# Lecture 21, Monday 16 Nov, HDD, TMY, CDD?

## Plan
- Demo of SMC functions
- Demo of TMY file

## Project Announcement
- We will load up projects from 4pm to 5pm Tuesday Nov 17th
- We will measure at the beginning of class on Wednesday Nov 18th

<!-- energy = power times time -->
<!-- relation of temperature inside to outside is delta T -->
<!-- delta T multiplied by the time step is the energy -->
<!-- you can pull the UA from the sum -->
<!-- delta T dt is the degree day -->

## Sage Math Cloud
- Markdown
    - Allows bold, lists, headings
- LaTeX
    - Allows math and greek symbols
- Code
    - Allows computations

<!-- create new ipython notebook -->
<!-- set kernel to python 3 -->
<!-- how to explain masking? -->


<!-- I made a notebook in SMC as an example -->


