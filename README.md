# Exceptional Shopping Cart Program

## Overview

This Java program implements an enhanced shopping cart system with robust exception handling. The system allows users to:
- Browse a catalog of market items
- Add/remove items from their shopping cart
- Calculate totals with tax
- Save and load cart summaries to/from files

The program demonstrates proper exception handling for various edge cases and invalid inputs.

## Key Features

### Market Catalog Operations
- `lookupProductByName()` - Finds product by name with exception handling
- `lookupProductById()` - Finds product by ID with input validation
- `addItemToMarketCatalog()` - Adds new items to the market catalog with parameter validation
- `getProductPrice()` - Retrieves product price with error checking

### Shopping Cart Operations
- `addItemToCart()` - Adds items to cart with size validation
- `removeItem()` - Removes items from cart with error checking
- `emptyCart()` - Clears the cart completely
- `checkout()` - Calculates total with tax
- `getCartSummary()` - Generates a formatted summary of cart contents

### File I/O Operations
- `saveCartSummary()` - Saves cart contents to a file
- `loadCartSummary()` - Loads cart contents from a file
- `parseCartSummaryLine()` - Helper method to parse file lines into cart items

## Exception Handling

The program handles various exceptional cases including:
- Invalid product IDs or names
- Negative sizes
- Full cart conditions
- File I/O errors
- Malformed data formats
- Null references

## Test Cases

The included test class `ExceptionalShoppingCartTester` verifies:
1. Product lookup methods handle invalid inputs
2. Market catalog additions validate parameters
3. Cart summary saving and loading operations
4. Edge cases for all major functionality

## How to Use

1. Compile all Java files
2. Run `ExceptionalShoppingCartTester` to verify functionality
3. Use the `ExceptionalShoppingCart` class methods to:
   - Build and manage shopping carts
   - Calculate totals
   - Save/load cart states
   - Look up product information

## File Format

Cart summaries are saved in the following format:
```
( quantity ) ItemName
( quantity ) AnotherItem
```

Example:
```
( 2 ) Apple
( 1 ) Banana
( 3 ) Milk
```

## Dependencies

- Java 8 or higher
- Standard Java libraries

## Author

Sai Gungurthi - CS 300 - University of Wisconsin-Madison
