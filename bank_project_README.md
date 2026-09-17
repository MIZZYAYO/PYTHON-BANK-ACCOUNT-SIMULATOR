# Bank Account Simulator

A command-line bank account simulator built in Python, using classes to model real
bank accounts — deposits, withdrawals, transaction history, and multiple accounts
managed through a simple menu system.

## Why a class?

A dictionary can store an account's data (balance, owner, history), but it can't
enforce rules about how that data changes. A class bundles the data AND the actions
that make sense for it (deposit, withdraw) together — so the only way to change an
account's balance is through methods that enforce the rules (e.g. you can't withdraw
more money than the account holds).

## Planned Features
- `BankAccount` class: stores owner, balance, and a full transaction history
- Deposit and withdraw money, with error handling (e.g. can't overdraw)
- Support for multiple accounts, managed via a dictionary
- Menu-driven program loop (create account / deposit / withdraw / check balance /
  view history / exit)
- Save and load accounts to/from a JSON file, so data persists between runs

## How to run
```bash
python3 bank_simulator.py
```

## Project structure
```
bank-account-simulator/
├── bank_simulator.py   # BankAccount class + menu program
├── accounts.json        # saved account data (created automatically)
└── README.md
```

## What I'm learning building this
- Classes and objects (`__init__`, `self`, methods)
- Managing multiple objects using a dictionary
- Error handling for invalid actions (overdrawing, invalid input)
- Converting custom objects to/from JSON for saving and loading data
- Building a menu-driven program loop
