# Error-Handling-in-Cpp
# Name: Rajeev Ramesh Reddy E
# PRN: 24070123081

Aim: To implement and demonstrate the concept of Exception Handling in C++ by writing programs that handle:

Software Used: Vs Code.

Theory:
Exception handling in C++ is a mechanism to manage runtime errors gracefully, ensuring program stability. It uses three keywords: try, catch, and throw. Code that might cause an error is placed inside a try block. If an exception occurs, it’s passed using throw, and handled by a matching catch block. This prevents abrupt termination and allows custom error messages or recovery logic. Exception handling improves robustness, especially in file I/O, memory allocation, and user input validation.

Syntax:
    
    #include <iostream>
    using namespace std;

    int main() {
    try {
        // Code that may throw an exception
        throw 100;  // Example: throwing an integer
    }
    catch (int e) {
        // Handling the exception
        cout << "Exception caught: " << e << endl;
    }

    return 0;
    }


Algorithm:

i) Algorithm: Age-Based Voting Eligibility (Exception Handling)

 1. Input Age
- Prompt the user to enter their age using `cin`.

 2. Try Block
- Use a `try` block to check if the entered age is less than 18.

 3. Throw Exception
- If `age < 18`, throw the age value as an exception.

 4. Catch Block
- Catch the thrown integer and display an error message indicating ineligibility for voting.

 5. Valid Age Output
- If age is 18 or above, print the age and confirm eligibility.


ii) Algorithm: Division with Exception Handling in C++

 1. Input Two Numbers
- Prompt the user to enter two floating-point numbers `n1` and `n2`.

 2. Try Block
- Use a `try` block to check if the second number `n2` is zero.

 3. Throw Exception
- If `n2 == 0`, throw the value to indicate a division error.

 4. Catch Block
- Catch the thrown float and display an error message indicating division by zero.

 5. Valid Division
- If `n2 != 0`, perform `n1 / n2` and display the result.


Conclusion:

This program effectively demonstrates exception handling in C++ by managing division-by-zero errors. Using `try`, `throw`, and `catch`, it ensures safe execution and user-friendly feedback. Such mechanisms enhance program reliability, prevent crashes, and are essential for robust applications involving user input, arithmetic operations, or unpredictable runtime conditions.
