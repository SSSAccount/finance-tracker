
# Personal Finance Tracker

A Python program for tracking personal finance transactions. It allows users to add, view, update, delete transactions, add transactions in bulk from a CSV file and display a summary of all transactions.


## Features

- Add a new transaction
- View transactions by category or view all transactions
- Add transactions in bulk from a CSV file
- Update existing transactions
- Delete a specific transaction
- Display a summary of one or all transactions

## Demo

https://github.com/SSSAccount/finance-tracker/assets/115540526/dda0211e-f3ed-41c4-89b5-e71f3da9cc49

## Requirements
- Python >= 3.12.1
- pip >= 24.0

## Installation

Ensure you are in the same directory as the requirements.txt file. Execute the following in the terminal.

```bash
pip install -r requirements.txt
```

Ensure you have also downloaded "finance_tracker.py", "helper.py", "financials.json" and "bulk.csv"

## Usage/Examples

Ensure "finance_tracker.py", "helper.py", "financials.json" and "bulk.csv" are in the same directory and then run 
```bash
python finance_tracker.py
```

 before using the following features:

1. **Adding Transactions**:
   - Choose option 1 from the main menu.
   - Follow the prompts to enter the transaction details such as category, amount, date and choice
   - Confirm the transaction to add it to the records.

2. **Viewing Transactions**:
   - Select option 2 from the main menu.
   - Choose a category to view transactions for that specific category.
   - To view all transactions, choose the "All" option.
   - Follow on-screen instructions to navigate through transactions.

3. **Adding Bulk Transactions**:
   - Make a copy of the bulk.csv to avoid any data loss as the program empties the file after adding the transactions (Optional)
   - Choose option 3 from the main menu.
   - Transactions will be added automatically from the file.

4. **Updating Transactions**:
   - Select option 4 from the main menu.
   - Follow the prompts to select the transaction to update which asks you for the ID of the transaction and the category of the transaction
   - Choose the aspect of the transaction to update (category, amount, date, choice).
   - Confirm the changes to update the transaction.

5. **Deleting Transactions**:
   - Choose option 5 from the main menu.
   - Follow the prompts to select the transaction to delete.
   - Confirm deletion to remove the transaction.

6. **Displaying Summary**:
   - Select option 6 from the main menu.
   - A summary of all transactions will be displayed, including net profit/loss, overall financial status, and the category with the most income and expense contributions.

7. **Exiting Program**:
   - Select option 7 from the main menu to exit the program.


## FAQ

#### 1. I tried to delete a newly added transaction but it says that it does not exist?

For now, the application can only delete already loaded transactions. To delete newly added transactions you have to run the application again.

#### 2. Why do I need an income and an expense to view the summary table instead of having only income or only expense?

For now, the application needs an income AND an expense in order to calculate the most contributing expense and income.


## Credits

[prettytable](https://github.com/jazzband/prettytable) - For creating summary tables and viewing transactions

[PyInputPlus](https://github.com/asweigart/pyinputplus) - For creating options and getting user input easier

[questionary](https://github.com/tmbo/questionary) - For 'Press any key to continue....'

[schema](https://github.com/keleshev/schema) - For checking the schema of bulk.csv
