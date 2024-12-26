# python-3


def calculate_discount(price, discount_percent):
    if discount_percent >= 20:
        return price * (1 - discount_percent / 100)
    else:
        return price
try:
    original_price = float(input(" 100: "))
    discount_percentage = float(input("25: "))
    
    # Calculate the final price
    final_price = calculate_discount(50, 10)
    
    # Display the result
    if final_price < original_price:
        print(f"The final price after applying the discount is: ${final_price:.2f}")
    else:
        print(f"No discount applied. The price remains: ${original_price:.2f}")
except ValueError:
    print("Please enter valid numeric values for the price and discount percentage.")
