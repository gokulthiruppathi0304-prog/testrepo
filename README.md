# Simple Interest Calculator

A simple, user-friendly command-line application built to calculate the simple interest earned or owed over a specific period.

## Description
This project calculates simple interest using the standard financial formula:
*SI = (P × R × T) / 100*

Where:
•⁠  ⁠*P* = Principal amount (the initial amount of money)
•⁠  ⁠*R* = Annual interest rate (in percentage)
•⁠  ⁠*T* = Time period (in years)

## Features
•⁠  ⁠Accepts user input for Principal, Rate, and Time.
•⁠  ⁠Handles decimal/floating-point inputs accurately.
•⁠  ⁠Displays calculated Simple Interest and the final Total Amount clearly.

## How to Run the Project
1.⁠ ⁠Clone this repository to your local machine:
   ⁠ bash
   git clone https://github.com
    ⁠
2.⁠ ⁠Navigate to the project directory:
   ⁠ bash
   cd YOUR_REPOSITORY_NAME
    ⁠
3.⁠ ⁠Run the Python script:
   ⁠ bash
   python calculator.py
    ⁠

## Example Usage
⁠ text
--- Simple Interest Calculator ---
Enter the Principal amount (\$): 1000
Enter the Annual Interest Rate (%): 5
Enter the Time period (in years): 2

--- Results ---
Simple Interest: \$100.00
Total Amount (Principal + Interest): \$1100.00
def calculate_simple_interest():
    print("--- Simple Interest Calculator ---")
    try:
        # Get user inputs
        principal = float(input("Enter the Principal amount ($): "))
        rate = float(input("Enter the Annual Interest Rate (%): "))
        time = float(input("Enter the Time period (in years): "))
        
        # Calculate interest and total
        interest = (principal * rate * time) / 100
        total_amount = principal + interest
        
        # Display results
        print("\n--- Results ---")
        print(f"Simple Interest: ${interest:.2f}")
        print(f"Total Amount (Principal + Interest): ${total_amount:.2f}")
        
    except ValueError:
        print("Error: Please enter valid numerical values.")

if _name_ == "_main_":
    calculate_simple_interest()
