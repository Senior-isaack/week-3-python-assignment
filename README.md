# week-3-python-assignment







question1 :# Function to calculate the final price after applying discount



def calculate_discount(price, discount_percent):
    # Check if discount is 20% or higher
    if discount_percent >= 20:
        # Apply discount
        discount_amount = (discount_percent / 100) * price
        final_price = price - discount_amount
        return final_price
    else:
        # No discount applied, return original price
        return price

# Main part of the program where we prompt the user for input
def main():
    # Get the original price and discount percent from the user
    price = float(input("Enter the original price of the item: "))
    discount_percent = float(input("Enter the discount percentage: "))
    
    # Calculate the final price using the function
    final_price = calculate_discount(price, discount_percent)
    
    # Print the final price
    print(f"The final price after applying the discount is: {final_price:.2f}" if discount_percent >= 20 else f"No discount applied. The price remains: {final_price:.2f}")





question2 ::User input and output:
Example Usage:
yaml



Enter the original price of the item: 100
Enter the discount percentage: 25
The final price after applying the discount is: 75.00


If the discount is less than 20%, it will print the original price:


Enter the original price of the item: 100
Enter the discount percentage: 10
No discount applied. The price remains: 100.00


