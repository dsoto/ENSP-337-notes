# Energy Modeling

## Modeling and Performance

- Code allows buildings to pass compliance for following a set of rules (prescriptive approach)
- Many predict an emphasis on building operation in the future
- This requires ways to observe and analyze data and make predctions

## Forward Models or Bottom-Up Models

- These models use measurements and properties of an object to make predictions about its behavior.
- Example: Estimate the UA product from the measurements and ideal thermal conductivities

## Backwards Models or Top-Down Models

- These models infer the properties of an object from observations of the objects behavior.
- Example: Estimate the UA product from the equilibrium temperature and the power input

## Intrusive and Non-Intrusive Data Collection

- Intrusive data collection requires changing the operating condition of the building, often in ways noticeable to the occupants.
- Non-intrusive data collection does not change the operation of a building.

## Slopes and Areas

- The key observables in thermal systems are temperature, power, and time.
- When graphed, the slopes and areas of these variables can provide important insight into building operation.

## Analytical Models

- For simple situations, we can write models using mathematical functions like the exponential function that describe building behavior.

## Computational Models

- For many physical situations, we start with a relationship for the slope of a curve and then use computational techniques to predict behavior.

## Setting Equalities

- Equalities are an indispensible tool for analysis
- We frequently use energy balance or setting energy quantities equal to generate useful equations
- What quantity are you setting equal?  (Energy, Temperature, Time?)
- What are the different ways you are expressing that quantity in your equation?  


# Computational Model

## Energy Balance

- First Law of Thermodynamics must be obeyed
- Where is the thermal energy in our system?

![](./figures/energy-balance.jpg)

## Warm-Up

- You are in a car with a watch and a clear view of the spedometer but
    the odometer is broken
- How do you estimate how far you have traveled?

## Draw a diagram

- How would you think about this graphically
- Graph total milage vs time
- Graph speed vs time

![](./figures/speed-distance.jpg)

![](./figures/distance-difference.jpg)

## Diagram

- Where are the thermal energy inputs and outputs in our system?

## Mathematical model

- Start by setting the energies equal to each other

$$ E_{in} = E_{out} $$

- Then add heat loss equation and thermal mass equation
- Can you solve to find the temperature?

![](./figures/difference-equations.jpg)

![](./figures/temperature-rise.png)


## Written notes

There are many notes from the board today necessary to understand the
lecture.

