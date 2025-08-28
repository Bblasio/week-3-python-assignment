# Week 3 Assignment
Overview
This Python program calculates the final price of an item after applying a discount, based on user input for the original price and discount percentage. The discount is applied only if the discount percentage is 20% or higher. The program is designed to be simple, user-friendly, and robust for handling basic discount calculations.
Purpose
The purpose of this assignment is to:

Practice writing Python functions with conditional logic.
Handle user input and perform basic arithmetic operations.
Format output to display currency values with two decimal places.

Code
Below is the complete Python code for the discount calculator:
def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        discount = price * (discount_percent / 100)
        return price - discount
    return price

# Prompt user for input
price = float(input("Enter the original price: "))
discount_percent = float(input("Enter the discount percentage: "))

# Calculate and print the final price
final_price = calculate_discount(price, discount_percent)
print(f"The final price is: ${final_price:.2f}")

How It Works

Function Definition:

The calculate_discount function takes two parameters:
price: The original price of the item (float).
discount_percent: The discount percentage (float).


If the discount percentage is 20% or higher, it calculates the discount amount (price * (discount_percent / 100)) and returns the discounted price (price - discount).
If the discount percentage is less than 20%, it returns the original price unchanged.


User Input:

The program prompts the user to enter:
The original price of the item.
The discount percentage.


Both inputs are converted to float to handle decimal values.


Output:

The program calls the calculate_discount function with the provided inputs.
The final price is printed, formatted to display two decimal places with a dollar sign (e.g., $10.00).



Requirements

Python Version: Python 3.x
Dependencies: None (uses standard Python libraries only)
Input Expectations:
The original price should be a positive number (integer or decimal).
The discount percentage should be a number (integer or decimal).
Note: The program does not include input validation, so users should ensure valid numeric inputs to avoid errors.



How to Run

Save the code in a file named discount_calculator.py.
Open a terminal or command prompt.
Navigate to the directory containing the file.
Run the program using the command:python discount_calculator.py


Follow the prompts to enter the original price and discount percentage.
The program will display the final price.

Expected Output
The program outputs the final price after applying the discount (if applicable), formatted as a currency value with two decimal places. Below are some example runs:
Example 1: Discount ≥ 20%
Enter the original price: 100
Enter the discount percentage: 25
The final price is: $75.00

Explanation: A 25% discount on $100 is $25, so the final price is $100 - $25 = $75.00.
Example 2: Discount < 20%
Enter the original price: 50
Enter the discount percentage: 10
The final price is: $50.00

Explanation: Since the discount percentage (10%) is less than 20%, no discount is applied, and the original price is returned.
Example 3: Decimal Inputs
Enter the original price: 99.99
Enter the discount percentage: 30.5
The final price is: $69.49


