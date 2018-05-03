# Economic Thickness of Insulation

If we consider both the annual cost of insulation and the annual cost of
energy, there is an optimal thickness where the cost of both is
minimized.

This is known as the economic thickness of insulation.

*Note: Place example from class notes here.*


We calculate

- The area of the cabin walls, floors, and ceiling
- The UA product of the cabin
- The yearly cost of the insulation
- The yearly cost of the natural gas
- The total cost of both

We observe that the total cost has a minimum at a given thickness of insulation.

# Area

We have an ideal cabin shaped like a cube with a dimension of 15 feet.  The area of the cube is
$$ A = 6 \cdot (15\ \textrm{ft})^2 $$


```python
area = 6 * (15 * u.feet)**2
area
```




1350 foot<sup>2</sup>



# Insulation

We are getting our insulation from Home Depot.

- R-Tech 320821
- 10.48 for a 4 foot by 8 foot sheet
- R-value of 3.85 per sheet

We can calculate the price per square foot and then multiply by the area of the cabin.

$$ price = A * \frac{\textrm{price per sheet}}{\textrm{area of sheet}} $$


```python
number_sheets = 1
price_insulation = 10.48 * u.dollar / (32 * u.foot**2) * number_sheets
area * price_insulation
```




442.125 dollar



# UA value

The UA value is the total area divided by the R value.  This is the same as the total area multiplied by the U-value.

$$ UA = \frac{A}{R} $$


```python
r_value = 3.85 * u.hour * u.foot**2 * u.delta_degF / u.BTU * number_sheets
area / r_value
```




350.649350649 btu/(delta_degF hour)




# Cost of Conserved Energy

The cost of conserved energy is cost of the equivalent purchase of energy to a conservation measure.

This allows us to compare this metric to the cost of energy.

$$ CCE = \frac{\textrm{annual extra investment cost}}{\textrm{annual energy savings}} $$

The key to this is a clear definition of the two scenarios you are comparing.
The cost is the difference in cost and the energy is the difference in energy between the two scenarios.

## Cost of conserved energy example

We can calculate the cost of conserved energy of adding an additional sheet of insulation.  To do this, we compare two scenarios, for example, the energy of only one sheet of insulation and then the energy of two sheets and the cost of the additional sheet.  Recall that our cost of energy in our previous calculation is 1 USD per therm.

### Scenario 1
- One sheet of insulation
- 50.5 MMBTU

### Scenario 2
- Two sheets of insulation
- 25.2 MMBTU
- 442 USD additional cost
- 44.20 USD yearly additional cost

$$ CCE = \frac{\textrm{annual extra investment cost}}{\textrm{annual energy avoided}} $$
$$ CCE = 44.20 USD/25.3 MMBTU = 0.17 USD/therm$$

### Scenario 4
- Four sheets of insulation
- 12.6 MMBTU

### Scenario 5
- Five sheets of insulation
- 10.1 MMBTU
- 44.20 USD yearly additional cost over scenario 4

$$ CCE = 44.20 USD / 2.5 MMBTU = 1.77 USD/therm $$

```python
(44.20 * u.dollar / (25.3e6 * u.BTU)).to(u.dollar/u.therm)
```

0.17 dollar/thm

```python
energy_price = 1e-5 * u.dollar / u.BTU
energy_price.to(u.dollar/u.therm)
```

1.0 dollar/thm

```python
(44.20 * u.dollar / (2.5e6 * u.BTU)).to(u.dollar/u.therm)
```

1.768 dollar/thm


# Cost of Conserved Carbon
