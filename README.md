# Splitwise-Style Expense Manager (C++ LLD)

A console-based Low-Level Design (LLD) implementation of a Splitwise-like Expense Manager built in **C++** using Object-Oriented Programming (OOP) principles and Design Patterns.

## 💡 Features

- Create users and groups
- Add users to groups
- Add group and individual expenses (Equal, Exact, and Percentage splits)
- Track group-specific and individual balances
- Settle payments between users
- Simplify group debts to minimize transactions
- Real-time notifications using the Observer pattern

## 🏗️ Design Patterns Used

- **Strategy Pattern**: For flexible split strategy (Equal, Exact, Percentage)
- **Observer Pattern**: For notifying users about new expenses and settlements
- **Singleton Pattern**: Central `Splitwise` manager instance
- **Factory Pattern**: For split strategy creation
- **Facade Pattern**: `Splitwise` acts as the main interface for managing operations

## 🧱 Class Structure

- `User`: Represents a person with balances and notification logic
- `Group`: Contains members, manages expenses, balances, and debt simplification
- `Expense`: Holds details of an expense (amount, payer, splits)
- `Split` & `SplitStrategy`: Abstracts different types of splits
- `Splitwise`: Main controller (Singleton) to manage users, groups, expenses
