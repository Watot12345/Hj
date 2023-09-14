#include <iostream>

// Function to calculate the factorial of a number
int factorial(int n) {
    if (n <= 1) {
        return 1;
    } else {
        return n * factorial(n - 1);
    }
}

int main() {
    int num;

    // Ask the user for input
    std::cout << "Enter a positive integer: ";
    std::cin >> num;

    if (num < 0) {
        std::cout << "Factorial is undefined for negative numbers." << std::endl;
    } else {
        // Calculate and display the factorial
        int result = factorial(num);
        std
