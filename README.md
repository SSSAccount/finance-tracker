
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

https://github-production-user-asset-6210df.s3.amazonaws.com/115540526/322344348-dda0211e-f3ed-41c4-89b5-e71f3da9cc49.mp4?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAVCODYLSA53PQK4ZA%2F20240415%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240415T055523Z&X-Amz-Expires=300&X-Amz-Signature=38eb7e39158527ff4ee77100fda057e33feccb228a73ce38e9d351a9256fee7b&X-Amz-SignedHeaders=host&actor_id=115540526&key_id=0&repo_id=786647793

## Requirements
- Python >= 3.12.1
- pip >= 24.0

## Installation

Ensure you are in the same directory as the requirements.txt file. Execute the following in the terminal.

```bash
pip install -r requirements.txt
```

Ensure you have also downloaded "finance_tracker.py", "helper.py", "financials.json" and create a new file called "bulk.csv" in the same directory

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
   - The bulk.csv file should look something like this:
   
      Salary,500,2024-02-29\
      Other, 300, 2024-02-29, Income 

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

#### 3. What are the supported categories?

The supported categories are:
Groceries, Salary, Utilities, Healthcare, Education and Other

The 'Other' category needs identification of whether it as an income or an expense. Any unsupported categories will be converted to the 'Other' category

## Credits

[prettytable](https://github.com/jazzband/prettytable) - For creating summary tables and viewing transactions

[PyInputPlus](https://github.com/asweigart/pyinputplus) - For creating options and getting user input easier

[questionary](https://github.com/tmbo/questionary) - For 'Press any key to continue....'

[schema](https://github.com/keleshev/schema) - For checking the schema of bulk.csv
