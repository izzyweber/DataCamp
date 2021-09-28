# SUMMARIZING THE TRIAL BALANCE
*This exercise would be part of Lesson 3.1: Summary Methods*
## Instructions
Summary functions in Pandas makes exploring financial data fast and easy. Let's use Python to get key information about a company's accounts, which are stored in a Pandas DataFrame. The head of the DataFrame looks like this:
|    |   acct_num | acct_type      | acct_name                     |   acct_balance |
|---:|-----------:|:---------------|:------------------------------|---------------:|
|  0 |       1000 | Current Assets | Accounts Receivable - 30 Days |           1111 |
|  1 |       1002 | Current Assets | Short Term Investments        |           1226 |
|  2 |       1004 | Current Assets | Inventory                     |           1785 |
|  3 |       1006 | Current Assets | Accounts Receviable - 90 Days |           1800 |
|  4 |       1008 | Current Assets | High Interest Cash Account    |            786 |
- Determine the total number of accounts in the trial balance.
```python
#Assume that each account is represented by one row in the trial balance
trial_balance["acct_balance"].____()
```
- Calculate the dollar value of total revenues.
```python
#We've used a Boolean mask create a new DataFrame, "revenues", which only contains the revenue accounts:
revenues = trial_balance[trial_balance["acct_type"]== "Revenue"]
#Sum up the total account balances for these revenue accounts
revenues["acct_balance"].____()
```
- Calculate the total dollar value for each account type.
```python
#Group the data by account type, then apply the correct summary function
trial_balance.____("acct_type").____()
```

## Solutions
- Determine the total number of accounts in the trial balance.
```python
#Assume that each account is represented by one row in the trial balance
trial_balance["acct_balance"].count()
```
>>> returns 85
- Calculate the dollar value of total revenues.
```python
#We've used a Boolean mask create a new DataFrame, "revenues", which only contains the revenue accounts:
revenues = trial_balance[trial_balance["acct_type"]== "Revenue"]
#Sum up the total account balances for these revenue accounts
revenues["acct_balance"].sum()
```
>>> returns 15312

- Calculate the total dollar value for each account type.
```python
#Group the data by account type, then apply the correct summary function
trial_balance.groupby("acct_type").sum()
```
>>> returns the below:

| acct_type             |   acct_num |   acct_balance |
|:----------------------|-----------:|---------------:|
| Cost of Goods Sold    |      35042 |           5354 |
| Current Assets        |      11110 |          11942 |
| Current Liabilities   |      20090 |          16388 |
| Long Term Assets      |      12418 |          13975 |
| Long Term Liabilities |       4202 |          10780 |
| Other Expense         |     187954 |          24498 |
| Revenue               |      20020 |          15312 |
| Shareholder's Equity  |      18030 |          13563 |
