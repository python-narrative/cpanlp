## Due to the existence of framing bias in natural language, we have developed Python narrative packages that includes [politicsnlp](https://pypi.org/project/politicsnlp/), [economynlp](https://pypi.org/project/economynlp/), [religionnlp](https://pypi.org/project/religionnlp/), [lawnlp](https://pypi.org/project/lawnlp/), and [cpanlp](https://pypi.org/project/cpanlp/), enabling us to communicate within a common framework and avoid misunderstandings caused by different frames of reference.

## Example
sales increased 12% compared with fourth quarter 2021:
  - North America segment sales increased 13% year-over-year to $93.4 billion, or increased 14% excluding changes in foreign exchange rates.
  - International segment sales decreased 8% year-over-year to $34.5 billion, or increased 5% excluding changes in foreign exchange rates.
  - AWS segment sales increased 20% year-over-year to $21.4 billion.
```python
sale1 = p.Sale(quarter="Q4",amount=93.4,unit="billion dollars",growth_rate=13%,year=2022,segment="North America")
sale2 = p.Sale(quarter="Q4",amount=34.5,unit="billion dollars",growth_rate=-8%,year=2022,segment="International")
sale3 = p.Sale(quarter="Q4",amount=21.4,unit="billion dollars",growth_rate=20%,year=2022,segment="AWS")
sales = [sale1, sale2, sale3]
total_sales = 0
for s in sales:
    total_sales += s.amount
    print(f"Segment: {s.segment}, Sale: {s.amount}")

print(f"Total Sales: {total_sales}")
```

<a href="https://cpanlp.com">
<img src="https://raw.githubusercontent.com/accounting-intelligent-ai/cpanlp/main/cpanlp.png" width = "250" height = "80" alt="logo" align=center />
</a>

Narrating [Accounting](https://cpanlp.com/overview/redefine)! using Python
Developed by **Cpanlp Intelligent Accounting Team** (c) 2023
[Github](https://github.com/accounting-intelligent-ai/cpanlp)

[![PyPI - Python Version](https://img.shields.io/static/v1?label=pypi&message=v1.2.40&color=blue)](https://pypi.org/project/cpanlp/)
[![Downloads](https://static.pepy.tech/badge/cpanlp/week)](https://pepy.tech/project/cpanlp)

## Install & Import
#### Dependencies
- scipy 
- numpy
- pandas
  
For detailed installation instructions, see the
[documentation](https://cpanlp.com/documentation).
```python
pip install cpanlp
import cpanlp as p
```

## Features
1. Accounting Item
```python
gold_asset = p.Asset(account="gold", debit=1000,date="2023-01-01")
print(gold_asset.bubble)
```
2. Information Asymmetry
```python
info = p.AsymmetricInformation(sender="investor", receiver="company_A", message="I am very interested in investing in your business", hidden_information="I have a limited budget")
info.get_advantage()
```
3. Entrepreneur
```python
john = p.Entrepreneur(name="John Smith",age=30,wealth=100000,utility_function=0, experience=5,company=LLC("Apple","Electronics",1000000),entrepreneurship=Entrepreneurship(leadership=9.0))
john.strive_for_excellence()
```
4. Strategy
```python
huawei = p.FinancialStrategy("huawei","defense",poison_pill(1000,0.1))
```

## Accounting Language Decorator :
```python
@prob(probability=0.7) #Estimate

@future_tense #Future Tense

side_effects=["financial instability","loss of reputation","decreased employee morale"]
@with_side_effects(side_effects=side_effects)#Side Effects 
```

## Accounting Exception :
```python
if abs(percent_change) > 10:
  raise AbnormalFluctuation(stock_name, percent_change)
```

## Module:
|  Module   | Content  |
|  :----:  | :----:  |
| **Abnormal**  | `Winner Curse`，`Bubble`|
| **Accounting Account**  | `Asset`，`Liability`，`Equity`，`Income`，`Cashflow` |
| **Business**  | `Main Business`，`Capacity` |
| ${\color{blue}Contract}$  | `Agreement`，`Arrangement`，`MOU`，`Commitment Letter`，`Lease`，`Loan Contract`，`Labor Contract`，`Financial Instrument` |
| **Cognitive**  | `BlackSwan`，`Grey Rhino`，`Herd Behavior` ，`Invisible Hand`，`Revolving Door` |
| **Control**  | `Voting Power`，`Commodity Control`，`Significant Influence` |
| **Culture**  | `Entrepreneurship`，`Craftsmanship`，`Business Philosophy` |
| ${\color{purple}Decorator}$| `Estimate` ，`Tense`，`Importance`，`With Effects`，`Validator`|
| **Department**  | `Board Of Directors` ，`Supervisory Board`|
| **Economic System** |  `Digital Economy` ，`Physical Economy` ，`Market Economy`，`Planned  Economy` |
| **Entity**  | `LLC(Limited Liability Company)`，`Partnership`，`Public  Company`，`SME(Small and medium-sized enterprises)`，`Conglomerate` |
| **Environment**  | `Economic Environment`，`Industry Environment`，`Credit Environment`，`Market Environment`|
| **Event**  | `Acquisition`，`Certification`，`Grants`，`Meeting`，`Resignation`，`Repurchase`，`Personnel`，`Registration`，`Shares`，`Lawsuit`，`StockHoldingIncrease` |
| ${\color{purple}Exception}$| `Abnormal Fluctuation`，`Bubble`，`Winner Curse`|
| **Information**  | `Signal`，`Speculative Information`，`Asymmetric Information` |
| **Incentive**  |   |
| **Institution**  |  |
| **Market**  | `Commodity`，`Goods`，`Market Structure`|
| **Person**  | ${\color{red}Consumer}$，`Employee`，`Entrepreneur`，`Manager`，`Investor`，`Partner`，`Shareholder`，`Supervisor`，`Creditor`，`Auditor`，`Beneficiary`，`Fiduciary`，`Craftsman` |
| **Policy**  | `AccountingPolicy`，`DividendPolicy` |
| **Project**  |  |
| **Pragmatics**  | `Promise` |
| **Risk** | |
| **StakerHolder**  | `Bank`，`Government`，`Media`，`Public`，`Rating Agency` |
| **Scheme**  | `Ponzi Scheme`，`ESOP`，`DebtRestructuringPlan` |
| **Strategy**  | `Long Term Strategy`，`Financial Strategy` |
| **Tax**  | `VAT(Value-Added Tax)`，`Consumption Tax`，`Personal Income Tax`，`Corporate Income Tax`，`RealEstate Tax`，`TransactionTax` |
| **Team**  |  |
| **Utility**  | |

## Accounting Gym-Env
<a href="https://pypi.org/project/cpagym/">
<img src="https://raw.githubusercontent.com/accounting-intelligent-ai/cpagym/main/cpagym.png" width = "200" height = "200" alt="logo" align=center />
</a>

Check out: https://cpanlp.com