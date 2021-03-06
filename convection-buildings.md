# Thought experiments
- What are the air currents in a warm house on a cold day?
- What are the air currents near the window of a warm house on a cold
    day?

## Activity
- Draw a picture of air currents on both sides of a window with a
    temperature difference
- Draw the temperature profile as a function of distance

## Lumped R-values
- $$R_{cvi}$$ inside r value
- $$R_{cvo}$$ outside r value

<!-- did we underestimate R effect last time -->

## Stack Effect
![](./figures/stack-effect-EFS.png)

## Wind Infiltration
![](./figures/wind-infiltration-EFS.png)

## Heat capacity of infiltration

Infiltration has an impact on energy required to heat or cool a home.
The air brought in from the outside must be warmed or cooled to the same
temperature as the inside air.  This energy adds an extra burden on the
heating system.

We calculate this by the usual $$ Q = mc \Delta T $$ for a mass of air.
We can however, convert this to a constant power if we assume that we
have a constant rate of infiltration.  Imagine that we know the mass of
air that enters each hour.  Dividing both sides by time gives us a power
on one side and a mass rate for $$m$$.

$$ Q_{inf} = m_{inf} c_{air} \Delta T $$

$$ \frac{Q_{inf}}{\Delta t} =\frac{ m_{inf}}{\Delta t}c_{air} \Delta T $$

Now we have a rate of infiltration in mass per unit time and a power.

$$ q_{inf} = r_{inf} c_{air} \Delta T $$

In the industry, we express this as air changes per hour ($$n$$) which is
essentially a rate of mass of air per unit time once we multiply by the
volume of air in the building and the density of air.

$$ q_{inf} = \rho_{air} c_{air} n V \Delta T $$

Here the temperature difference is between the inside and outside air.

![](./figures/infiltration-equation-EFS.png)

## Heat Loss
![](./figures/home-heat-loss-EFS.png)


## Learning Objectives
- Perform convection calculations

## Temperature profile with air films
![](./figures/window-rcv.png)

## Window Temperatures
![](./figures/window-temps.png)

## R-values

- $$R_{cvi}$$ = 0.68 hr-sqft-F/BTU
- $$R_{cvo}$$ = 0.17 hr-sqft-F/BTU
- 3/16 inch of glass, k = 5.5 BTU-in/hr-sqft-F

## Questions

- What is the inside temperature of the glass?
- What is the heat loss for a 2 foot by 3 foot window?



<!-- quiz went super long and we will do these calculations on monday -->
<!-- how will you figure this out in five years -->

## Method
- What is your overall strategy?
- How do you collect your starting values for your estimates?
- How will you organize your calculation so that you get it correct?
- How will you organize your calculation so that others understand it?

## Measurements
- Inside 70 degrees F
- Outside 25 degrees F
- 3/16 inch thick glass
- k = 5.5 BTU-in/hr-sqft-F

## Multiple Resistances
![](./figures/multiple-resistances.png)


