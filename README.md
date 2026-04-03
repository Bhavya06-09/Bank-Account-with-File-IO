## Complete banking system with persistent data storage.
## Features
Account class:
├── deposit() - add money
├── withdraw() - remove money
├── getBalance() - check funds
└── File IO - save/load account.txt
## Menu
1=Deposit 2=Withdraw 3=Balance 4=Save 5=Load 0=Exit
## File Handling
**PrintWriter** → saves name + balance to `account.txt`
**Scanner + File** → loads account data on restart
## Demo Flow
Deposit 500 → Balance: 1500 → Save → Restart
Load → Balance: 1500 (persists!)
## Tech Stack
java.io.*
├── PrintWriter (write)
├── Scanner + File (read)
├── try-with-resources (auto-close)
└── Exception handling
## Run
javac BankAccountIO.java
java BankAccountIO
**Creates account.txt** - data survives program restart!

