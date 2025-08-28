# Week 3 Assignment

# Overview
This Python program calculates the final price of an item after applying a discount, based on user input for the original price and discount percentage.  
The discount is applied only if the discount percentage is 20% or higher.  
The program is designed to practice key programming skills, including function creation, conditional logic, user input handling, and formatted output.  
# Purpose
This assignment focuses on developing the following skills:

1. Practice writing Python functions with conditional logic to control program flow.  
2. Handle user input and perform basic arithmetic operations to compute discounts.  
3. Format output to display currency values with two decimal places for clarity.  

Code
```
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
```

How It Works
The program addresses the assignment objectives as follows  

1. Writing Python Functions with Conditional Logic:  
2. Defines a function calculate_discount that takes two parameters: price (float) and discount_percent (float).  
3. Uses conditional logic (if discount_percent >= 20) to determine whether to apply a discount:  
4. If the discount percentage is 20% or higher, calculates the discount (price * (discount_percent / 100)) and returns the discounted price (price - discount).  
5. Otherwise, returns the original price unchanged.  


Handling User Input and Performing Arithmetic Operations:  
Prompts the user to input the original price and discount percentage using input().  
Converts inputs to float to support decimal values.  
Performs arithmetic operations in the calculate_discount function to compute the discount and final price.  


Enter the original price and discount percentage when prompted.  
View the final price displayed by the program.  

Example 1: Lets use the following values  
Discount ≥ 20%  
Enter the original price: 100  
Enter the discount percentage: 25  
The final price is: $75.00  



