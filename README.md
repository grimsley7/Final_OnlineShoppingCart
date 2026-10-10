# Online Shopping Cart Final Project

This project is a Python-based Online Shopping Cart system developed as the final Principles of Programming application. The program uses object-oriented programming with two core classes, `ItemToPurchase` and `ShoppingCart`, and a menu-driven interface for managing cart items.

## Project Overview

The system allows a user to:
- initialize a shopping cart with a customer name and date
- add items with a name, description, price, and quantity
- review item details before adding them to the cart
- remove items by name
- change item quantities
- change item prices
- display item descriptions
- display the full shopping cart and total cost

The program also includes input validation to reduce invalid entries and improve usability.

## Class Structure

### `ItemToPurchase`
Stores:
- item name
- item description
- item price
- item quantity

Methods:
- `print_item_cost()`
- `print_item_description()`

### `ShoppingCart`
Stores:
- customer name
- current date
- list of cart items

Methods:
- `add_item()`
- `find_item()`
- `remove_item()`
- `modify_item()`
- `update_price()`
- `get_num_items_in_cart()`
- `get_num_items()`
- `get_cost_of_cart()`
- `print_total()`
- `print_descriptions()`

## Menu Options

- `a` = Add item to cart
- `r` = Remove item from cart
- `c` = Change item quantity
- `p` = Change item price
- `i` = Output items' descriptions
- `o` = Output shopping cart
- `q` = Quit

## Features Added

To make the program more practical and easier to use, I added:
- confirmation messages for add, remove, and modify actions
- a review step before an item is added to the cart
- duplicate item handling with a user prompt
- quantity change to `0` removes the item
- alphabetical sorting when printing the cart and descriptions
- a price update option for correcting mistakes after an item has already been added
- validation for names, prices, quantities, dates, and yes/no responses

## Currency Formatting

Prices are handled using Python's `Decimal` type instead of `float` so currency values stay more accurate. This helps prevent rounding issues and keeps prices like `$7.19` from being displayed incorrectly. All prices and totals are displayed with two decimal places.

## File Included

- `online_shopping_cart.py` – main Python program

## How to Run

1. Open the Python file in Visual Studio Code or another IDE.
2. Run the program.
3. Enter the customer name and date when prompted.
4. Use the menu to manage the shopping cart.

## Author

Shemecca Grimsley
