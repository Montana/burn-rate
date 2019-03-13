![logo](logo.png)

## Prowl's burn rate

Burn Rate is a simple library for computing a weekly expenditure from a list of bills over a monthly and yearly cycle for Prowl, but don't be afraid to use at it your company as well! 

The term burn rate can also refer to how quickly individuals spend their money, particularly their discretionary income.

## Assumptions

Burn rate makes the following assumptions about Prowl & your startup:  

* You organize your finances on a weekly basis
* Every "pay week" starts on Thursday

## Usage

*output.py* implements a simple commandline tool to generate a burn rate.
it is run via
```python
output.py data.json
```

data.json is a set of information regarding your outputs, in the form:
```json
{
 "weekly": {
  "weekly_project": {
   "amount": 100,
   "day": "Monday" # unused
  },
  ... # etc
},
 "monthly": {
  "some_project": {
   "date": "01",
   "amount": 100
  },
  ... # etc
 },
 "yearly": {
  "yearly_project: {
   "date": "January 01",
   "amount": 100
  },
  ... # etc
 }
}
```

