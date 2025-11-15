📌 Project Overview

This is a simple ATM Machine simulation written in Java.
It demonstrates core Object-Oriented Programming (OOP) concepts such as:

Encapsulation

Interfaces

Implementation classes

User interaction through console

Basic banking operations (withdraw, deposit, check balance, mini statement)

The project allows a user to:

✔ Login with ATM number and PIN
✔ Check available balance
✔ Withdraw money
✔ Deposit money
✔ View a Mini Statement

📂 Project Structure
ATM Project
│
├── Atm.java
├── AtmMain.java
├── AtmOperationInterf.java
└── AtmOperationImpl.java

📘 File Descriptions
1. Atm.java

This class represents the data model for the ATM account.
It contains:

Account number

ATM PIN

Account balance

Getter & Setter methods

It is used to store and access user account details safely (encapsulation).

2. AtmOperationInterf.java

This is the interface that defines the operations supported by the ATM:

viewBalance()

withdrawAmount(double amount)

depositAmount(double amount)

viewMiniStatement()

This ensures any ATM implementation must follow these method signatures.

3. AtmOperationImpl.java

This class implements the interface and contains the actual logic.

Operations include:

✅ Check Balance

Prints the current account balance.

✅ Withdraw Money

Checks if the balance is sufficient

Deducts the amount

Adds entry to mini statement

✅ Deposit Money

Adds amount to balance

Adds entry to mini statement

✅ Mini Statement

Prints last transactions using a HashMap.

This file contains the main working logic of the ATM.

4. AtmMain.java

This is the main executable class.

Prompts the user to enter:

ATM number

PIN

Verifies login credentials

Displays a menu:

1. View Available Balance
2. Withdraw Amount
3. Deposit Amount
4. View Mini Statement
5. Exit


Executes operations using AtmOperationImpl

This file controls the entire user flow.

▶ How to Run

Compile all .java files:

javac *.java


Run the main class:

java AtmMain

✨ Features

Object-oriented design

Secure login check

Realistic ATM operations

Mini-statement tracking

Simple console interface
