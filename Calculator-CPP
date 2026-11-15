
#include <iostream>
#include <iomanip>
#include <limits>
using namespace std;

// Function Declarations
void displayMenu();
void addition(double a, double b);
void subtraction(double a, double b);
void multiplication(double a, double b);
void division(double a, double b);
void showWelcome();
void showExitMessage();

// Main Function
int main()
{
    int choice;
    double num1, num2;
    char continueChoice;

    showWelcome();

    do
    {
        displayMenu();

        cout << "\nEnter your choice: ";

        if (!(cin >> choice))
        {
            cout << "\nInvalid input! Enter a number.\n";
            cin.clear();
            cin.ignore(numeric_limits<streamsize>::max(), '\n');
            continue;
        }

        if (choice == 5)
        {
            break;
        }

        if (choice < 1 || choice > 5)
        {
            cout << "\nInvalid choice! Please try again.\n";
            continue;
        }

        cout << "\nEnter the first number: ";
        cin >> num1;

        if (cin.fail())
        {
            cout << "Invalid number!\n";
            cin.clear();
            cin.ignore(numeric_limits<streamsize>::max(), '\n');
            continue;
        }

        cout << "Enter the second number: ";
        cin >> num2;

        if (cin.fail())
        {
            cout << "Invalid number!\n";
            cin.clear();
            cin.ignore(numeric_limits<streamsize>::max(), '\n');
            continue;
        }

        cout << "\n========== RESULT ==========\n";

        switch (choice)
        {
            case 1:
                addition(num1, num2);
                break;

            case 2:
                subtraction(num1, num2);
                break;

            case 3:
                multiplication(num1, num2);
                break;

            case 4:
                division(num1, num2);
                break;
        }

        cout << "============================\n";

        cout << "\nDo you want to continue? (Y/N): ";
        cin >> continueChoice;

    } while (continueChoice == 'Y' ||
             continueChoice == 'y');

    showExitMessage();

    return 0;
}

// Welcome Message
void showWelcome()
{
    cout << "\n";
    cout << "************************************\n";
    cout << "*                                  *\n";
    cout << "*       BASIC CALCULATOR           *\n";
    cout << "*       C++ MINI PROJECT           *\n";
    cout << "*                                  *\n";
    cout << "************************************\n";
}

// Display Menu
void displayMenu()
{
    cout << "\n========== MAIN MENU ==========\n";
    cout << "1. Addition       (+)\n";
    cout << "2. Subtraction    (-)\n";
    cout << "3. Multiplication (*)\n";
    cout << "4. Division       (/)\n";
    cout << "5. Exit\n";
    cout << "===============================\n";
}

// Addition
void addition(double a, double b)
{
    double result = a + b;

    cout << fixed << setprecision(2);
    cout << "\nOperation: Addition\n";
    cout << "Number 1: " << a << endl;
    cout << "Number 2: " << b << endl;
    cout << "Result: " << result << endl;
}

// Subtraction
void subtraction(double a, double b)
{
    double result = a - b;

    cout << fixed << setprecision(2);
    cout << "\nOperation: Subtraction\n";
    cout << "Number 1: " << a << endl;
    cout << "Number 2: " << b << endl;
    cout << "Result: " << result << endl;
}

// Multiplication
void multiplication(double a, double b)
{
    double result = a * b;

    cout << fixed << setprecision(2);
    cout << "\nOperation: Multiplication\n";
    cout << "Number 1: " << a << endl;
    cout << "Number 2: " << b << endl;
    cout << "Result: " << result << endl;
}

// Division
void division(double a, double b)
{
    cout << fixed << setprecision(2);

    cout << "\nOperation: Division\n";

    if (b == 0)
    {
        cout << "Error: Cannot divide by zero!\n";
    }
    else
    {
        double result = a / b;

        cout << "Number 1: " << a << endl;
        cout << "Number 2: " << b << endl;
        cout << "Result: " << result << endl;
    }
}

// Exit Message
void showExitMessage()
{
    cout << "\n************************************\n";
    cout << "*  Thank you for using calculator! *\n";
    cout << "*          PROGRAM ENDED           *\n";
    cout << "************************************\n";
}
