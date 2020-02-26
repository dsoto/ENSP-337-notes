# Heating and Cooling Degree Days

# Concepts

- Heating Degree Days
- Cooling Degree Days
- UA Product
- Balance Point
- Base Temperature
- California Climate Zones
- Typical Meteorological Year (Synthesized Data)
- Historical Data

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

## Base Temperature

This is the temperature we use to construct our temperature differences.
It is related to the thermostat setting in the buildings.

## California Climate Zones

California designates 16 climate zones and compiles data for them to aid in climate-aware building design.

PG&E maintains
[a training document](https://www.pge.com/myhome/edusafety/workshopstraining/pec/toolbox/arch/climate/index.shtml)
detailing these zones.

## Typical Meteorological Year (Synthesized Data)

Typical Meteorological Year (TMY) constructs a typical data set by taking the most typical month from the last several years and mixing them together in a data set.

## Historical Data

These are the actual recorded data from weather stations that have been compiled for analysis.

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

# Heating Degree Day Calculations

The basic steps of a calculation are

- Obtain time series of outside temperature and base temperature
- Create temperature differences
- Discard negative temperature differences
- Sum temperature differences

You must of course ensure that your calculations respect units and dimensions.

## HDD and CDD methods

- Integration method
    - Uses high-resolution data to compute degree-days for each hour of day
- Minimum--Maximum--Average approximations
    - Uses low resolution data that may only have high and low daily temperatures

# Data Sources

- [Cal Adapt Degree Days](https://cal-adapt.org/tools/degree-days/)
- [TMY3 Synthetic Data](https://rredc.nrel.gov/solar/old_data/nsrdb/1991-2005/tmy3/by_state_and_city.html)
- [NOAA Historical Weather Data](https://www.ncdc.noaa.gov/cdo-web/search)

# Further Reading
- [Degree Days Calculation Details](https://www.degreedays.net/calculation)
- Energy for Sustainability Chapter 6 Energy Efficiency for Buildings
- Building Science, Pohl, Chapter 3 and 4
