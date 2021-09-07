#include <iostream>
#include <ctype.h>
/*
Forex Bureau Currency Exchange Calculator - Solution Requirements
An interactive program to accept name, telephone number,
national card number
The telephone must be verified to ensure it corresponds
with the number of digits (10 digits)
Let a user choose their preferred currency and the exchange format
eg. Cedi-to-Pound or Pound-to-Cedi
The currencies must cover USD, Euro, Pound, Yuan, Rand, Cedi
Print the currency equivalent for the chosen conversion.
Display the name, contact, national card number, and the
conversion summary of the forex activity.
*/
using namespace std;

bool isNumber(char c)
{
   if (isdigit(c))
    return true;
        return false;
}

int main()
{
   string firstName, lastName, telephone;
   int cardNumber, choice, digit=0;

    cout << "Enter your first name: ";
    cin >> firstName;
    cout << "Enter your last name: ";
    cin >> lastName;
    cout << "Enter your national number: ";
    cin >> cardNumber;
    while (1)
    {
    cout << "Enter your telephone number: ";
    cin >> telephone;

        for (int i = 0; i < telephone.size(); i++)
        {
            if (isNumber(telephone[i]))
            {
                digit++;
            }
        }

        if (digit == 10)
        {
            break;
        }
        else
        {
            cout << "Wrong Input.\n";
        }
    }
    cout << "Choose your preferred currency exchange format. \n";
    cout << "1. USD-to-Euro \n2. USD-to-Pound\n";
    cout << "3. USD-to-Yuan \n4. USD-to-Rand\n";
    cout << "5. USD-to-Cedi\n";
    cout << "6. Euro-to-USD \n7. Euro-to-Pound\n";
    cout << "8. Euro-to-Yuan \n9. Euro-to-Rand\n";
    cout << "10. Euro-to-Cedi\n";
    cout << "11. Pound-to-USD \n12. Pound-to-Euro\n";
    cout << "13. Pound-to-Yuan \n14. Pound-to-Rand\n";
    cout << "15. Pound-to-Cedi\n";
    cout << "16. Yuan-to-USD \n17. Yuan-to-Euro\n";
    cout << "18. Yuan-to-Pound \n19. Yuan-to-Rand\n";
    cout << "20. Yuan-to-Cedi\n";
    cout << "21. Rand-to-USD \n22. Rand-to-Euro\n";
    cout << "23. Rand-to-Pound \n24. Rand-to-Yuan\n";
    cout << "25. Rand-to-Cedi\n";
    cout << "26. Cedi-to-USD \n27. Cedi-to-Euro\n";
    cout << "28. Cedi-to-Pound \n29. Cedi-to-Yuan\n";
    cout << "30. Cedi-to-Rand\n\n\n";

    cin >> choice;

    switch (choice)
    {
    case 1:
        cout << " 1 USD = 0.84 Euro";
        break;
    case 2:
        cout << "1 USD = 0.72 Pounds";
        break;
    case 3:
        cout << "1 USD = 6.46 Yuan";
        break;
    case 4:
        cout << "1 USD = 14.24 Rand";
        break;
    case 5:
        cout << "1 USD = 6.06 Cedis";
        break;
    case 6:
        cout << "1 Euro = 1.19 USD";
        break;
    case 7:
        cout << "1 Euro = 0.86 Pounds";
        break;
    case 8:
        cout << "1 Euro = 7.67 Yuan";
        break;
    case 9:
        cout << "1 Euro = 16.90 Rand";
        break;
    case 10:
        cout << "1 Euro = 7.19 Cedis";
        break;
    case 11:
        cout << "1 Pound = 1.38 USD";
        break;
    case 12:
        cout << "1 Pound = 1.17 Euro";
        break;
    case 13:
        cout << "1 Pound = 8.94 Yuan";
        break;
    case 14:
        cout << "1 Pound = 19.71 Rand";
        break;
    case 15:
        cout << "1 Pound = 8.39 Cedi";
        break;
    case 16:
        cout << "1 Yuan = 0.15 USD";
        break;
    case 17:
        cout << "1 Yuan = 0.13 Euro";
        break;
    case 18:
        cout << "1 Yuan = 0.11 Pound";
        break;
    case 19:
        cout << "1 Yuan = 2.20 Rand";
        break;
    case 20:
        cout << "1 Yuan = 0.94 Cedis";
        break;
    case 21:
        cout << "1 Rand = 0.07 USD";
        break;
    case 22:
        cout << "1 Rand = 0.059 Euro";
        break;
    case 23:
        cout << "1 Rand = 0.051 Pounds";
        break;
    case 24:
        cout << "1 Rand = 0.45 Yuan";
        break;
    case 25:
        cout << "1 Rand = 0.43 Cedis";
        break;
    case 26:
        cout << "1 Cedi = 0.17 USD";
        break;
    case 27:
        cout << "1 Cedi = 0.14 Euro";
        break;
    case 28:
        cout << "1 Cedi = 0.12 Pounds";
        break;
    case 29:
        cout << "1 Cedi = 1.07 Yuan";
        break;
     case 30:
        cout << "1 Cedi = 2.35 Rand";
        break;
     default:
        break;
    }

    cout << "\n\n\n===============================\n";
    cout << "Name: " <<firstName <<" " <<lastName <<endl;
    cout << "Contact: " <<telephone <<endl;
    cout << "National Card Number: " <<cardNumber <<endl;
    cout << "Conversion Summary: \n";

    switch (choice)
    {
    case 1:
        cout << " 1 USD = 0.84 Euro";
        break;
    case 2:
        cout << "1 USD = 0.72 Pounds";
        break;
    case 3:
        cout << "1 USD = 6.46 Yuan";
        break;
    case 4:
        cout << "1 USD = 14.24 Rand";
        break;
    case 5:
        cout << "1 USD = 6.06 Cedis";
        break;
    case 6:
        cout << "1 Euro = 1.19 USD";
        break;
    case 7:
        cout << "1 Euro = 0.86 Pounds";
        break;
    case 8:
        cout << "1 Euro = 7.67 Yuan";
        break;
    case 9:
        cout << "1 Euro = 16.90 Rand";
        break;
    case 10:
        cout << "1 Euro = 7.19 Cedis";
        break;
    case 11:
        cout << "1 Pound = 1.38 USD";
        break;
    case 12:
        cout << "1 Pound = 1.17 Euro";
        break;
    case 13:
        cout << "1 Pound = 8.94 Yuan";
        break;
    case 14:
        cout << "1 Pound = 19.71 Rand";
        break;
    case 15:
        cout << "1 Pound = 8.39 Cedi";
        break;
    case 16:
        cout << "1 Yuan = 0.15 USD";
        break;
    case 17:
        cout << "1 Yuan = 0.13 Euro";
        break;
    case 18:
        cout << "1 Yuan = 0.11 Pound";
        break;
    case 19:
        cout << "1 Yuan = 2.20 Rand";
        break;
    case 20:
        cout << "1 Yuan = 0.94 Cedis";
        break;
    case 21:
        cout << "1 Rand = 0.07 USD";
        break;
    case 22:
        cout << "1 Rand = 0.059 Euro";
        break;
    case 23:
        cout << "1 Rand = 0.051 Pounds";
        break;
    case 24:
        cout << "1 Rand = 0.45 Yuan";
        break;
    case 25:
        cout << "1 Rand = 0.43 Cedis";
        break;
    case 26:
        cout << "1 Cedi = 0.17 USD";
        break;
    case 27:
        cout << "1 Cedi = 0.14 Euro";
        break;
    case 28:
        cout << "1 Cedi = 0.12 Pounds";
        break;
    case 29:
        cout << "1 Cedi = 1.07 Yuan";
        break;
     case 30:
        cout << "1 Cedi = 2.35 Rand";
        break;
     default:
        break;
    }
    return 0;
}
