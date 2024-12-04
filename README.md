# Calculator

## Overview
This project is a programmer's calculator that performs various conversions and calculations involving different numerical bases and floating-point representations. It uses linked lists to manage dynamic data structures for these operations.

## Features
1. **Base Conversion**: Convert a decimal number to binary, octal, hexadecimal, and BCD (Binary-Coded Decimal).
2. **Signed Conversion**: Convert a decimal number with a sign to a 16-bit two's complement representation.
3. **Floating-Point Conversion**: Convert a real number to its IEEE 754 floating-point representation for both single precision (float) and double precision (double).

## Functions

### Stack Operations
- `void push(int data, struct Node **top)`: Pushes an integer onto the stack.
- `void pop(struct Node **top)`: Pops an integer from the stack.
- `void ClearNode(struct Node **top)`: Clears the entire stack.
- `void PrintNode(struct Node *top)`: Prints the contents of the stack.

### Linked List Operations
- `void InsertLast(float target, struct Node** start)`: Inserts a float at the end of the linked list.
- `void DeleteFirst(struct Node** start)`: Deletes the first node of the linked list.
- `int length(struct Node *top)`: Returns the length of the linked list.

### Conversion Functions
- `int power(int base, int expoente)`: Returns the result of raising a base to an exponent.
- `int BinToDecimal(struct Node *top)`: Converts a binary number stored in a stack to its decimal representation.
- `void DecimalToBaseX(int numeroConvertido, int baseNumerica, struct Node **top)`: Converts a decimal number to a specified base and stores it in the stack.
- `void AddBits(int numeroBits, struct Node **top)`: Adds a specified number of bits (zeros) to the stack.
- `void DecimalToBCD(int numeroConvertido, struct Node **top)`: Converts a decimal number to its BCD representation.
- `int LastDigitOneInBin(struct Node *top)`: Returns the position of the last digit one in a binary number stored in a stack.
- `void TwosComplement(int lastOnePos, struct Node**top)`: Converts a binary number to its two's complement representation.

### Floating-Point Operations
- `int FractionBin(float fracao, struct Node **top, int mantissaBits)`: Converts the fractional part of a float to binary and stores it in the stack.
- `void AddExponent(int exp, int bias, struct Node **top)`: Adds the exponent to the stack with a specified bias.
- `void AddSignal(char signal, struct Node **top)`: Adds the sign bit to the stack.

## Usage
Compile the project using the following command:
```sh
gcc src/*.c -I include -o programa
```
Run the executable:
```sh
./programa
```
Author
Miguel de Sousa Batista