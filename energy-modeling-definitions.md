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

# Baselines

Buildings often use more energy than what the architect expects.
This is due to many factors including human behavior and the way the building was actually constructed.

The practice of measuring the performance of a building over time is often called "baselining" of a building.

# Gathering data

- Cumulative vs incremental readings

# Analyzing data

- How do you move from a cumulative reading to an incremental reading?
- Spedometer vs Odometer
- Discrete differences on the computer

# Comparing performance

- How do you compare to previous performance
- How do you account for differences in the weather
- For differences in occupancy?
- What do linear multivariate regression models look like?

# Predicting Energy Use

- How much energy do you expect a building to use?
- What depends on the design of the building?
- What depends on the behavior of the occupants?