This Java code implements a simple banking system that allows you to manage bank accounts. Here’s a breakdown of the key components:

Classes
Bank: This class manages multiple accounts.

Attributes:
accounts: A HashMap that stores account numbers as keys and Account objects as values.
Methods:
addAccount(String accountNumber, String customerName, double balance): Creates a new Account object and adds it to the accounts map.
displayAccountInfo(String accountNumber): Displays details of an account if it exists; otherwise, it prints "Account not found!".
performTransaction(String accountNumber, double amount): Adds the specified amount to the account's balance if the account exists. If it doesn't, it prints an error message.
Account: Represents a single bank account.

Attributes:
accountNumber: The account's unique identifier.
customerName: The name of the account holder.
balance: The current balance of the account.
Methods:
getAccountNumber(), getCustomerName(), and getBalance(): Getters for the account details.
deposit(double amount): Increases the account balance by the specified amount.
BankingSystem: This is the main class containing the main method, which serves as the entry point for the program.

It creates an instance of the Bank, adds a couple of accounts, performs transactions, and displays account information.
Flow of Execution
When the program starts, it creates a Bank object.
It adds two accounts: John Doe's with a balance of $1000.0 and Jane Smith's with $1500.0.
It performs a transaction of $500.0 on John Doe's account, which increases his balance to $1500.0.
It tries to perform a transaction of $200.0 on a non-existent account (number "103"), which triggers an error message.
Finally, it displays the account information for both John Doe and Jane Smith.

Example Output
Here’s a sample output based on the provided transactions:

Transaction successful. Updated balance: $1500.0
Account not found!
Account Number: 101
Customer Name: John Doe
Balance: $1500.0
Account Number: 102
Customer Name: Jane Smith
Balance: $1500.0

Summary
Overall, this code is a basic demonstration of object-oriented programming in Java, encapsulating data (account details) and behavior (account management) in a simple banking application.
