# Lecture 01

## Your learning goals

- Form groups of two or three and discuss the following
- Why are you taking this class?
- What are your learning goals for this class?

<!-- skills vs credential -->


## Learning Objectives

- Understand how this class will function
- Understand the larger context for thermal energy




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
# Lecture 04
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


# Lecture 22, Wed 18 Nov, HDD, TMY, CDD

## Announcements
- 5pm at the HUB dialogue on the campus community

## Weighing of Ice Cubes

## Quiz 6




# Lecture 23, Mon 23 Nov 2015, Economic Cost of Insulation

## Announcements

## Economic Cost of Insulation
- How much insulation should we apply to a home?

## Thought experiment
- You have a small cabin in a cold area
- You are insulating the walls with rigid insulation
- How many layers should you apply?

## Calculation
- What is the area of the cabin?
- What is the cost of insulation?
- What does the insulation cost if you pay back over 10 years?

## Calculation
- What is the yearly heating need for the cabin?
- How much does this energy cost each year?

## Calculation
- How does this combined cost vary with the number of sheets?



# Lecture 24, Mon 30 Nov 2015, Conserved cost of Energy

## Announcements
- Project Presentation Signups
- Final Exam Team Signups

## Conserved Cost of Energy

The conserved cost of energy is cost of the equivalent purchase of
energy to a conservation measure.

This allows us to compare this metric to the cost of energy.

$$ CCE = \frac{\textrm{annual extra investment cost}}{\textrm{annual energy avoided}} $$

The key to this is a clear definition of the two scenarios you are
comparing.  The cost is the difference in cost and the energy is the
difference in energy between the two scenarios.


## CCE
- calculate for the additional sheets of insulation on our cabin
- write up calculation better and put in course notes
- fire up sage math cloud

# Lecture 25, Projects, 2 Dec 2015


