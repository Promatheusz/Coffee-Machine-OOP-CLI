# Introduction
The Coffee Machine OOP project is a Python application that simulates a coffee machine. 
It allows users to select different types of coffee, processes the payment, and dispenses 
the coffee if sufficient resources are available.

# Run 
```bash
python main.py
```
# Classes
## Menu
The Menu class is responsible for managing the coffee menu. 
It provides methods to get the available menu items and to find a specific drink by name.
### Methods
- get_items(): Returns a string of available menu items.
- find_drink(order_name): Returns the drink object if it exists in the menu.

## CoffeeMaker
The CoffeeMaker class handles the coffee machine's resources and operations. 
It checks if there are enough resources to make a drink and deducts the resources when a drink is made.
### Methods
- report(): Prints the current resource values.
- is_resource_sufficient(drink): Returns True if there are enough resources to make the drink, otherwise False.
- make_coffee(order): Deducts the required resources to make the drink.

## MoneyMachine
The MoneyMachine class manages the financial transactions. It processes the payment and keeps track of the total money earned.
### Methods
- report(): Prints the current money earned.
- make_payment(cost): Returns True if the payment is successful, otherwise False.
