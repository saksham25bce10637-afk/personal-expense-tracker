●  Project Tile - PERSONAL EXPENSE TRACKER


● Overview of the project - The provided Python code implements a Human-Driven Expense Tracker delivered as a Command-Line Interface (CLI) application.
Primary Objective
The core goal of this project is to create a robust system for users to log and analyze their personal financial transactions (expenses). It provides persistent data storage and leverages data processing tools to deliver useful financial insights.
Key Features Summary
Data Persistence: Uses the sqlite3 library to create and manage an embedded database (ledger_records.db), ensuring all transaction data is saved permanently.
Implemented by the DataPilot class.
Business Logic: Manages the process of validation, recording, retrieval, and aggregation of expense data.
Implemented by the BudgetOverseer class.
Financial Reporting: Generates a detailed textual summary of total spending aggregated by category.
Uses pandas for efficient grouping and calculation.
Visualization: Creates a Pie Chart using matplotlib to visually break down where the user's money was spent across different categories.
This project is a great example of a three-tier architecture, successfully separating Data Handling (Persistence), Business Logic (Aggregation/Reporting), and Presentation (CLI) into distinct classes.



● Features - Key Features of the Personal Expense Tracker
1. Core Expense Management
Simple Transaction Logging: Easily record new expenses, including amount, date, and category, through a user-friendly command-line or graphical interface.
Categorization System: Predefined and custom categories (e.g., Food, Housing, Transport) to accurately classify and track spending types.
Data Persistence: Securely save all expense records to a file (CSV, JSON, or a lightweight database like SQLite) for reliable future access and analysis.


2. Reporting and Analysis
Summary Reports: Generate aggregated reports showing total spending for specific time periods (e.g., daily, weekly, monthly, annually).
Spending Visualization: (If using a library like Matplotlib or Plotly) Create simple charts or graphs to visualize spending distribution across categories or trends over time.
Filtering and Sorting: Ability to filter expenses by date range, category, or amount, and sort records for quick review.


3. Utility and Usability
Expense Editing/Deletion: Functionality to modify or remove existing transaction records to correct errors or update details.
Data Export: Option to export tracked data into common formats (e.g., CSV) for external analysis or backup purposes.
Search Functionality: Quickly find specific transactions using keywords in the description or notes field.


● Technologies/tools used - The Human-Driven Expense Tracker utilizes a variety of Python libraries, both standard and external, to manage data persistence, processing, and visualization effectively.
Data and Backend Technologies
Python: Serves as the core programming language for the entire application, housing all the logic and structure.
sqlite3: This standard Python module is critical for data persistence. It allows the application to create and manage an embedded, disk-based SQLite database (ledger_records.db), where all transaction records are securely stored and retrieved.


● Steps to install & run the project - Installation and Setup
Step 1: Install Required Libraries
Before running the code, you need to ensure the two external data science libraries, pandas and matplotlib, are installed in your Python environment.
Open your terminal or command prompt and run the following command:
pip install pandas matplotlib
This command uses Python's package installer (pip) to download and install both libraries.

Step 2: Save the Code
Copy the entire Python code you provided and save it as a file named tracker.py (or any .py file name) on your computer.

Step 3: Execute the Project
Navigate to the directory where you saved the tracker.py file using your terminal:
cd /path/to/your/saved/file
Once in the correct directory, run the script using the Python interpreter:
python tracker.py
🚀 Running the Application Loop
Upon successful execution, the application will start its main loop and present you with the primary menu:
Welcome to the Human-Driven Expense Tracker CLI!


--- Main Menu ---
1. Record a New Expense
2. View All Past Records
3. View Category Spending Report
4. EXIT APPLICATION


● Instructions for testing - Your menu choice (1-4): 
Key Execution Steps
Select 1 (Record a New Expense): The application will prompt you for the amount, category, description, and whether the expense is recurring. This action creates a new record in the ledger_records.db SQLite file.
Select 3 (View Category Spending Report): This option will display the text summary and generate the category_spending_pie_chart.png image



● Screenshots (optional but recommended) - here are the screenshots

The screenshots of the input
<img width="1070" height="614" alt="Screenshot 2025-11-23 013527" src="https://github.com/user-attachments/assets/632c038d-4167-48e3-bfa0-015dedb52e6a" />
<img width="1050" height="726" alt="Screenshot 2025-11-23 013552" src="https://github.com/user-attachments/assets/dce857a3-1c06-46b1-9dc0-17b32170e772" />
<img width="985" height="731" alt="Screenshot 2025-11-23 013616" src="https://github.com/user-attachments/assets/40422914-e5d9-4cc3-9385-ef5c378cd720" />
<img width="984" height="724" alt="Screenshot 2025-11-23 013635" src="https://github.com/user-attachments/assets/edfc6b28-a6dd-4ecf-9dcd-0b266f36bde0" />
<img width="1059" height="725" alt="Screenshot 2025-11-23 013657" src="https://github.com/user-attachments/assets/63b9d184-47e2-4039-a240-0b5afab0e1ab" />
<img width="918" height="705" alt="Screenshot 2025-11-23 013751" src="https://github.com/user-attachments/assets/dedcccf1-f1ea-48ea-b527-d0eeed926e6d" />
<img width="759" height="596" alt="Screenshot 2025-11-23 013819" src="https://github.com/user-attachments/assets/95343263-c2c3-46ae-b38b-0fcb4b8315d6" />
<img width="744" height="325" alt="Screenshot 2025-11-23 013913" src="https://github.com/user-attachments/assets/4713dc81-f321-4313-9127-d9aa29b1ede1" />


The screenshots of the output
<img width="811" height="612" alt="Screenshot 2025-11-23 014019" src="https://github.com/user-attachments/assets/edec9c39-26ba-498b-8547-63cc8043f14a" />
<img width="805" height="713" alt="Screenshot 2025-11-23 014040" src="https://github.com/user-attachments/assets/0432d801-bd0e-4005-909e-b11600d3ba75" />
