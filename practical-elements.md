# Practical Elements

# Questions

- How do we apply the physics of heat transfer in practice?
- What elements of buildings can lower energy usage?

# Learning Objectives
- Calculate the energy used when a specified building element is used.

# Concepts

- Heating Degree Days
- Cooling Degree Days
- UA Product
- Balance Point
- Index

## UA Product

- power per temperature difference
- Total Heat loss coefficient (ASHRAE)
- Overall Heat Loss Factor (EFS)

This tells you how much thermal power must be delivered in order to
maintain a desired temperature difference.

## Balance Point

Any building has several internal sources of thermal energy.  The
lighting, occupants, and appliances all provide heat to the building.
The balance point tells us what temperature difference the building will
have between the outside temperature and the inside temperature without
providing any energy from the heating system.

## Heating Degree Days

This metric provides a simple way to distill a year's worth of temperature data to a single number that is useful for energy estimations.

Recall that we can estimate the heat power for a structure's envelope if we know the UA value and the temperature difference between the inside and the outside.

$$ q = UA\Delta T $$

We assume for some interval of time $$\Delta T$$ that the temperature is constant.
Over that period of time, the energy moving from the inside of the envelope to the outside is

$$ E = UA \Delta T \Delta t $$

Since outside temperatures change fairly slowly, we can estimate the energy by assuming the temperature is constant over the course of an hour.
We call each temperature reading $$\Delta T_i$$ and sum over our period of time (often a year).

$$ E_{year} = \Sum_{i=1}^{8760} UA \Delta T_i \Delta t $$

Since the UA value doesn't change over time, we can write the UA outside of the sum.

$$ E_{year} = UA \Sum_{i=1}^{8760} \Delta T_i \Delta t $$

The quantity in the sum is the degree days.
Degree days are often tabulated using weather data and assumptions about the inside temperature of a building.
We can also calculate degree day quantities if our assumptions are significantly different from the usual assumptions.



# Reading
- Energy for Sustainability Chapter 6 Energy Efficiency for Buildings
- Building Science, Pohl, Chapter 3 and 4

## Walls
- Conductive heat flow

## Insulation
- Conductive heat flow

## Windows
- Reflectivity
- Emissivity
- Spectral response

## Water Heating
- Heat capacity

## Refrigeration
- Metrics for CDD
- Metrics for volume
- Thermodynamic cycle

## Heat Pumps
- Thermodynamic cycle

## Time Step Calculations

If we have a known thermal mass surrounded by a known insulating
exterior and begin to heat the mass, what will the change in temperature
look like?

## Spectrally Selective Materials

In a cold climate, it would be advantageous to be able to absorb
sunlight very efficiently, but radiate heat very inefficiently.  What
properties would such a material have?

## Maximum Temperature

- Given a heater emitting a constant power, what is the equilibrium
    temperature for a home?
- For simple cases, we can estimate this from the UA product

$$ q = U A \Delta T $$

$$ \Delta T = T_{inside} - T_{outside} = q/UA $$

## Box Experiment

- Our temperature difference is about 13C (38C - 25C)
- The power in that trial was about 47 watts
- The UA product is then 3.6 watts per degree C
