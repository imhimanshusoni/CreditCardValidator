<!--
# CreditCardValidator
A C++ program to check whether a credit card is valid or not using Luhn algorithm.
>The Luhn algorithm, also known as the modulus 10 or mod 10 algorithm, is a simple checksum formula used to validate a variety of identification numbers, such as credit card numbers, IMEI numbers, Canadian Social Insurance Numbers.

![image](https://user-images.githubusercontent.com/71898557/211466632-4eea5d0f-1cc7-4630-82e0-6173cec69f2c.png)
-->

# Credit Card Validator

This project is a C++ program that can validate credit card numbers using Luhn's algorithm. Luhn's algorithm is a simple checksum formula that is used to verify various identification numbers, such as credit card numbers, IMEI numbers, social insurance numbers, etc.

The program takes a credit card number as input and checks if it is valid or not. It does this by following these steps:

- Drop the last digit of the number, which is the check digit.
- Starting from the rightmost digit, double the value of every second digit.
- If doubling a digit results in a two-digit number, add the digits of the product to get a single-digit number.
- Sum all the digits of the number.
- Calculate the check digit by subtracting the sum from the next multiple of 10.
- Compare the check digit with the original last digit of the number. If they match, the number is valid; otherwise, it is invalid.

The program uses a function called `checkLuhn` that implements Luhn's algorithm and returns a boolean value indicating whether the input number is valid or not. The function takes a string parameter representing the credit card number and uses a loop to iterate over each digit. It uses arithmetic operations and modulus to perform the calculations and comparisons.

The program also uses a function called `isValidLength` that checks if the input number has a valid length for a credit card number. The function takes a string parameter representing the credit card number and returns a boolean value indicating whether the length is between 13 and 19 digits, which are the common lengths for most credit card issuers.

The main function of the program prompts the user to enter a credit card number and validates it using both `checkLuhn` and `isValidLength` functions. It displays a message indicating whether the number is valid or not. It also handles invalid inputs such as empty strings or non-numeric characters.

The program is written in C++ and can be compiled and run using any standard C++ compiler and IDE. It does not require any external libraries or dependencies. It is a simple and useful project that demonstrates how to use Luhn's algorithm to validate credit card numbers in C++.

## Screenshots
<img src='https://user-images.githubusercontent.com/71898557/232845944-8f244553-b6af-4760-924b-84b384758898.png' width='49%'> <img src='https://user-images.githubusercontent.com/71898557/232846065-fc1ee5aa-1b2c-4a4d-8284-484d99df765e.png' width='49%'>
