# Heating and Cooling Degree Days

# Concepts

- Heating Degree Days
- Cooling Degree Days
- UA Product
- Balance Point
- California Climate Zones

## Heating and Cooling Degree Days

These metrics provide a simple way to distill a year's worth of temperature data to a single number that is useful for energy estimations.
We will see that the energy to heat and cool is proportional to the heating degree days (HDD) and cooling degree days (CDD) values.

## UA Product

We recall that the UA product is the overall thermal conductance of the house telling us how much power must be applied to maintain a given temperature difference.

## Selected UA Values

|                       |              |                  |                 |
|-----------------------|--------------|------------------|-----------------|
| 1500 square foot home | 500 BTU/hr/F | 7.7 BTU/sf/day/F | EFS Chapter 6   |
| ETC walls only        | 150 W/K      |                  | Class Estimates |


<!-- - power per temperature difference
- Total Heat loss coefficient (ASHRAE)
- Overall Heat Loss Factor (EFS) -->

## Balance Point

Any building has several internal sources of thermal energy.
The lighting, occupants, and appliances all provide heat to the building.
The balance point tells us what temperature difference the building will
have between the outside temperature and the inside temperature without
providing any energy from the heating system.

## California Climate Zones

California designates 16 climate zones and compiles data for them to aid in climate-aware building design.

PG&E maintains
[a training document](https://www.pge.com/myhome/edusafety/workshopstraining/pec/toolbox/arch/climate/index.shtml)
detailing these zones.

# Heating Degree Day Derivation

Recall that we can estimate the heat power for a structure's envelope if we know the UA value and the temperature difference between the inside and the outside.

$$ q = UA\Delta T $$

We assume for some interval of time $$\Delta T$$ that the temperature is constant.
Over that period of time, the energy moving from the inside of the envelope to the outside is

$$ E = UA \Delta T \Delta t $$

Since outside temperatures change fairly slowly, we can estimate the energy by assuming the temperature is constant over the course of an hour.
We call each temperature reading $$\Delta T_i$$ and sum over our period of time (often a year).

$$ E_{year} = \sum_{i=1}^{8760} UA \Delta T_i \Delta t $$

Since the UA value doesn't change over time, we can write the UA outside of the sum.

$$ E_{year} = UA \sum_{i=1}^{8760} \Delta T_i \Delta t $$

The quantity in the sum is the degree days.
Degree days are often tabulated using weather data and assumptions about the inside temperature of a building.
We can also calculate degree day quantities if our assumptions are significantly different from the usual assumptions.

# Further Reading
- Energy for Sustainability Chapter 6 Energy Efficiency for Buildings
- Building Science, Pohl, Chapter 3 and 4
