# Postfix Expression Calculator

This is a simple calculator implemented using the `Calculator` class, which processes postfix expressions (e.g., "4 5 + 1 2 * - 5 /"). The calculator uses a stack to evaluate the postfix expression and displays the step-by-step process in a tabular format.

## Class Description

### Calculator

The `Calculator` class takes a postfix expression as input and processes the operators and operands from left to right. It uses a stack to calculate the postfix expression and prints the output in a table format, showing columns for "Method", "Return Value", and "Stack Contents".

## Usage

1. Clone this repository
2. Compile and run the main class (`Calculator`)
3. Enter a postfix expression as input
4. The calculator will process the expression and display the step-by-step evaluation in a table format

## Example

Input:
4 5 + 1 2 * - 5 /

Output:
Method | Return Value | Stack Contents
push(4) | | 4
push(5) | | 4, 5
pop() + pop()| 9 | 9
push(1) | | 9, 1
push(2) | | 9, 1, 2
pop() * pop()| 2 | 9, 2
pop() - pop()| 7 | 7
push(5) | | 7, 5
pop() / pop()| 1.4 | 1.4

## Contributing

If you would like to contribute to this project, please follow these steps:

1. Fork the repository
2. Create a new branch with your feature or bug fix
3. Commit your changes and push them to your fork
4. Create a pull request to this repository

## License

This project is released under the MIT License. Please see the `LICENSE` file for more details.
