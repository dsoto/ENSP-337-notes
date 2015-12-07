# Economics Fundamentals

Finances dictate most energy decisions and we choose the technology that
is the least cost according to some criteria.  In this chapter we
introduce a few criteria that are commonly used.

<!--
grab from 338 notes and work
use luenberger text and examples from ENSP 438
-->


## Learning Objectives

- Calculate equivalent sums of money using discount rates

## Concepts
- Time Value of Money
- Equivalence and Comparison Principle
- Net Present Value (NPV)
- Future Value
- Discounting
- Discount rate
- Interest rate


## Equivalence principle
- Given a choice between money now and money later, most demand a larger
  value at a later date
- When someone is indifferent between sum 1 now and sum 2 at a fixed
  later date, the sums are considered equivalent
- This equivalence can be expressed using a discount rate


## Discount rate vs. Interest rate

- Discount rate usually refers to personal preferences
- Interest rate is usually a real rate charged by a bank

## Monthly vs. Yearly interest rates

- Many types of loans advertise a yearly interest rate, but charge
    interest monthly.
- The yearly interest rate is the APR or annual percentage rate
- To find the monthly rate divide this by twelve
- $i$ is the annual percentage rate
- $n$ is the number of periods in months

$$ FV = PV (1 + i/12)^{n} $$



## Cash flow diagrams
![Cash Flow Diagram](./figures/cash-flow.png)


## NPV Spreadsheet Example
<!-- create a net present value calculation -->
<!-- show by hand and with NPV function -->

- Excel considers first value in the NPV function to be year 1

## Loan Spreadsheet Example

- You can arrive at a loan payment by trial and error in a spreadsheet.




## Learning Objectives

- Able to use the internal rate of return (IRR) to quantify an energy investment
- Able to use the capital recovery function (CRF) to estimate a loan
    payment
- Recognize cost of conserved energy (CCE) and  cost of conserved carbon


## Review

- Discounting
- Time Value of Money
- NPV


## Time Value of Money
## Concepts
- Internal Rate of Return (IRR)
- Capital Recovery Function (CRF)
- Spreadsheet solution for CRF
- Inflation


## Internal Rate of Return
- Tells us at what interest rate a cash flow has a net present value of
  zero
- We will look at this on a spreadsheet
- This doesn't have a closed-form solution
- Usually solved by a computer


# Inflation

## Inflation

- The cost of goods usually rises over time
- This rate is monitored by the [Consumer Price Index](http://www.bls.gov/cpi/)
- As prices rise, the value of money decreases


## Inflation

$$ 1 + r_0 = \frac{1+r}{1+f} $$

- $r_0$ is the effective rate of interest
- $r$ is the nominal rate of interest
- $f$ is the inflation rate

For small inflation rates,

$$ r_0 \approx r - f $$


## CRF Spreadsheet Example
<!-- show by hand and with PMT function -->
<!-- compare to calculator online -->

- Excel PMT
- Excel IRR


<!-- ## CRF Scripting Example -->
<!--  -->
<!-- &#45; np.pmt() -->
<!-- &#45; np.irr() -->



# Future Value
## Equivalence principle
- Given a choice between money now and money later, most demand a larger
  value at a later date
- When someone is indifferent between sum 1 now and sum 2 at a fixed
  later date, the sums are considered equivalent
- This equivalence can be expressed using a discount rate


## Discount Rate and Net Present Value
$$\textrm{Present Value (USD)} =
\frac
{\textrm{Future Amount (USD)}}
{(1 + \textrm{Discount Rate})^{\textrm{number of years in future}} }$$

$$P = \frac {F} {(1 + i)^{n} }$$


## Present Value Notation
Single payment
$$ PV = \frac{C}{(1+i)^n} $$

Stream of payments
$$ PV = C_0 +
        \frac{C_1}{1+i} +
        \frac{C_2}{(1+i)^2} +
        \dots +
        \frac{C_N}{(1+i)^N}$$

Compact notation
$$ PV = \sum_{n=0}^{N} \frac{C_n}{(1+i)^n}$$


## Discount rate vs. Interest rate

- Discount rate usually refers to personal preferences
- Interest rate is usually a real rate charged by a bank

## Monthly vs. Yearly interest rates

- Many types of loans advertise a yearly interest rate, but charge
    interest monthly.
- The yearly interest rate is the APR or annual percentage rate
- To find the monthly rate divide this by twelve
- $i$ is the annual percentage rate
- $n$ is the number of periods in months

$$ FV = PV (1 + i/12)^{n} $$



## Cash flow diagrams
![Cash Flow Diagram](./figures/cash-flow.png)


## NPV Spreadsheet Example
<!-- create a net present value calculation -->
<!-- show by hand and with NPV function -->

- Excel considers first value in the NPV function to be year 1

## Loan Spreadsheet Example

- You can arrive at a loan payment by trial and error in a spreadsheet.




# Present Value

# Net Present Value

# Internal Rate of Return

## IRR
Finding the IRR is the equivalent of asking, here is a loan, what was
the interest rate you got?


# Capital Recovery Function

## Capital Recovery Factor
Suppose we make a loan.  We want to know what the yearly payment is so
that the present value of all payments is equal to the loan amount.

This formula allows us to calculate this payment.

$$CRF = \frac {i(1+i)^n}{(1+i)^n-1}$$



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




# Conserved Cost of Energy

The conserved cost of energy is cost of the equivalent purchase of
energy to a conservation measure.

This allows us to compare this metric to the cost of energy.

$$ CCE = \frac{\textrm{annual extra investment cost}}{\textrm{annual energy savings}} $$

The key to this is a clear definition of the two scenarios you are
comparing.  The cost is the difference in cost and the energy is the
difference in energy between the two scenarios.

## Conserved cost of energy example

We can calculate the conserved cost of energy of adding an additional sheet of insulation.  To do this, we compare two scenarios, for example, the energy of only one sheet of insulation and then the energy of two sheets and the cost of the additional sheet.  Recall that our cost of energy in our previous calculation is 1 USD per therm.

### Scenario 1
- One sheet of insulation
- 50.5 MMBTU

### Scenario 2
- Two sheets of insulation
- 25.2 MMBTU
- 442 USD additional cost
- 44.20 USD yearly additional cost

$$ CCE = \frac{\textrm{annual extra investment cost}}{\textrm{annual energy savings}} $$
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




