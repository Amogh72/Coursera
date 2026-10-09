# Simple Interest Calculator

A simple interest calculator works out the interest earned or paid on a principal amount over a period of time at a fixed annual rate. Unlike compound interest, simple interest is calculated only on the original principal.

## Formula

```
Simple Interest (SI) = (P × R × T) / 100
Total Amount (A)     = P + SI
```

| Symbol | Meaning                          | Example     |
|--------|----------------------------------|-------------|
| P      | Principal (initial amount)       | ₹10,000     |
| R      | Rate of interest per year (%)    | 5           |
| T      | Time period (in years)           | 3           |

## Example

For a principal of ₹10,000 at 5% per year for 3 years:

```
SI = (10000 × 5 × 3) / 100 = ₹1,500
A  = 10000 + 1500          = ₹11,500
```

## Inputs

1. **Principal amount** – a positive number
2. **Annual interest rate (%)** – a positive number
3. **Time period (years)** – a positive number

## Outputs

- Simple interest
- Total amount (principal + interest)

## Sample Program (Python)

```python
def simple_interest(principal, rate, time):
    return (principal * rate * time) / 100

p = float(input("Enter principal amount: "))
r = float(input("Enter annual interest rate (%): "))
t = float(input("Enter time period (years): "))

si = simple_interest(p, r, t)
print(f"Simple Interest: {si:.2f}")
print(f"Total Amount: {p + si:.2f}")
```

### Sample Run

```
Enter principal amount: 10000
Enter annual interest rate (%): 5
Enter time period (years): 3
Simple Interest: 1500.00
Total Amount: 11500.00
```

## How to Run

1. Make sure Python 3 is installed.
2. Save the sample program as `simple_interest.py`.
3. Run it with: `python simple_interest.py`
4. Enter the principal, rate and time when prompted.

## Validation Rules

- All inputs must be numeric.
- Principal, rate and time should be greater than zero.
- If time is given in months, convert it to years by dividing by 12.

## Use Cases

- Estimating interest on short-term loans
- Calculating returns on fixed deposits that pay simple interest
- Learning basic financial mathematics
