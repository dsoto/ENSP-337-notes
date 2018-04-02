# Midterm 2 Review

We want to estimate the conserved cost of energy for the replacement of the blinds in the ETC.

## Scenario one:

- Business as Usual (BAU)
- Blinds remain closed
- Natural gas consumption remains the same

## Scenario two:

- Blinds replacement
- We can open blinds and get solar gain
- Natural gas consumption lowered by solar gain
- Yearly cost for blinds replacement loan

The conserved cost of energy

$$ CCE = \frac{\textrm{annual additional cost}}
              {\textrm{annual energy avoided}} $$

is calculated from the cost and energy differences between these two scenarios.

## Annual additional cost:

We need to know the following things to estimate the annual additional cost:

- initial cost of the blinds
- the interest rate of the loan
- the length of the loan

## Energy Avoided

- area of the window
- orientation of the window
- solar irradiance (power per area) in our location

We can get data for the solar irradiance from the
[NREL Solar Radiation Data Manual for Buildings](http://rredc.nrel.gov/solar/pubs/bluebook/).
We will use the data for Sacramento and assume similar weather patterns and insolation.

## Total Energy Required for Heating

We don't need this to calculate the CCE but we might be interested in the total heating energy per year so we can see how significant the solar gain is toward the budget.

<!-- note we have a large discrepancy here in the ETC between the UA DD product and the gas bill -->

<!-- Is the UA value for the ETC in the Beeler report? -->


# Computations

## Solar Gain


The ETC has a large clerestory south facing window that is approximately 6 feet high and 18 feet wide.

We assume that the insolation on a south-facing vertical surface is 1426 BTU per square foot per day.

We assume the window transmits 71 percent of the solar radiation.

## What is the solar gain through this window?

For this we multiply the power per unit area incident on the window by the area.


```python
from pint import UnitRegistry
u = UnitRegistry()

transmission = 0.71
# NREL data sacramento south shaded transmitted double glazing
insolation = 610 * u.BTU / u.foot**2 / u.day
area = 6 * u.foot * 18 * u.foot
solar_gain = insolation * transmission

def pprint(string, value):
    print((string + ' {:0.3g}').format(value))

pprint('insolation', insolation.to(u.kWh/u.meter**2/u.day))
pprint('solar gain', solar_gain*area)
pprint('solar gain', (solar_gain*area).to(u.kWh/u.day))
pprint('solar gain', (solar_gain*area).to(u.therm/u.day))


```

    insolation 1.92 kilowatt_hour / day / meter ** 2
    solar gain 4.68e+04 btu / day
    solar gain 13.7 kilowatt_hour / day
    solar gain 0.468 thm / day


## Avoided cost

This estimation suggests that the window allows us to offset approximately 1 therm of energy.
Assuming efficient combustion of natural gas, this is about 1 therm of natural gas.
At 1 dollar per therm, we avoid about a dollar per day during days that would require heating.

## Conserved Cost of Energy

We need to estimate both the annual cost and the annual fuel avoided.

The annual cost is calculated from the CRF loan cost

- $15K replacement
- 5 year loan at 8%

The annual fuel avoided would be about 1 dollar for each day requiring heating.
We could use the weather data, or we could estimate over the three months using heating.

If we find our conserved cost of energy is very high despite using optimistic estimation assumptions, we can stop there.
If we find it is close, we can refine our model.


```python
import numpy as np

loan = 15e3
periods = 5
rate = 0.08

annual_cost = -np.pmt(rate, periods, loan)
print(-np.pmt(rate, periods, loan))
print(rate * (1+rate)**periods/((1+rate)**periods - 1) * loan)
```

    3756.8468185
    3756.8468185025463


We take the annual cost per year and divide by the estimated avoided energy per year to get a energy cost estimate.


```python
annual_cost / ((solar_gain*area).to(u.therm/u.day) * 180 * u.day)
```




44.62097371640933 1/thm


