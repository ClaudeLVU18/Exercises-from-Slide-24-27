//CODE FOR EXERCISES ON SLIDE 24-27 LECTURE 6


//Odd or Even number checker with user input and input error checking
#include <iostream> //allows for variables to be loaded
#include <string> // allows string to be used
#include <stdlib.h>


using namespace std;
  
int main()
{   
    cout << "\n\nInput a number to check whether it is an odd or even number: \n\n";
    int num;
    cin >> num;
    
    
    if(cin.fail()) // to check for user input error
    {
    cin.clear();
    cout << "\n\nERROR: Sorry, that is not a valid number. \n" << endl;
    cin>>num;
    }
    if(!cin.fail()) //allows for the code to end if user input error is present.

    if((num & 1) == 0)
    {
        cout << "\n\n" << num << " is an even number.";
    }
    else
    {
        cout << "\n\n" << num << " is an odd number.";
        
    }
    cin.get();

    return 0; 
}


//Positive, Negative, Zero number checker with user input and input error checking
#include <iostream> //allows for variables to be loaded
#include <string> // allows string to be used
#include <stdlib.h>


using namespace std;
  
int main()
{   
    cout << "\n\nInput a number to check whether is value is positive, negative an odd or even number: \n\n";
    int num;
    cin >> num;

    if(cin.fail()) // to check for inappropriate input error
    {
    cin.clear();
    cout << "\n\nERROR: Sorry, that is not a valid number. \n" <<endl;
    cin>>num;
    }
    if(!cin.fail()) //allows for the code to end if user input error is present.

    if(num > 0)
    {
        cout << "\n\nThe number inputted is a positive number.\n\n" << endl;
    }
    else if(num < 0)
    {
        cout << "\n\nThe number inputted is a negative number.\n\n" << endl;
    }
    else
    {
        cout << "\n\nThe number inputted is 0.\n\n" << endl;
    }
    cin.get();
                                                           
    return 0; 
}

//Profit Loss Checker
#include <string> // allows string to be used
#include <stdlib.h>


using namespace std;
  
int main()
{   
    cout << "Enter Purchase price:  \nAED ";
    int buy;
    cin >> buy;
    if(cin.fail()) 
    {
    cin.clear();
    cout << "\n\nERROR: Sorry, that is not a valid number. \n" <<endl;
    cin>>buy;
    }
    if(!cin.fail()) 

    cout << "\nEnter Sale price: \nAED ";
    int sell;
    cin >> sell;

    
    if(cin.fail())
    {
    cin.clear();
    cout << "\n\nERROR: Sorry, that is not a valid number. \n" <<endl;
    cin>>sell;
    }
    if(!cin.fail())
    
    if(sell > buy)
    {
        cout << "\n\nSale profit";
        cout << "\nProfit: AED "<< sell - buy;
    }
    else if(sell == buy) //if no profit nor loss has been made.
    {
        cout << "\n\nBreak-even point.\n\n";
    }
    else
    {
        cout << "\n\nSale loss";
        cout << "\nLoss: AED " << buy - sell; 
    }
                                                           
    return 0; 
}

//Shape Identifier
#include <string> // allows string to be used
#include <stdlib.h>


using namespace std;
  
int main()
{   
    cout << "With a shape having around 3 to 10 sides in mind, input its number of sides: ";
    int side;
    cin >> side;

    if(cin.fail())
    {
    cin.clear();
    cout << "\n\nERROR: Sorry, invalid number input. \n" <<endl;
    cin>>side;
    }
    if(!cin.fail())

    switch (side)
    {
        case 3:
        cout << "\n\nA shape with 3 sides would be a Triangle.\n" << endl;
        break;
        case 4:
        cout << "\n\nA shape with 4 sides would be a Square/Quadrilateral.\n" << endl;
        break;
        case 5:
        cout << "\n\nA shape with 5 sides would be a Pentagon.\n" << endl;
        break;
        case 6:
        cout << "\n\nA shape with 6 sides would be a Hexagon.\n" << endl;
        break;
        case 7:
        cout << "\n\nA shape with 7 sides would be a Heptagon.\n" << endl;
        break;
        case 8:
        cout << "\n\nA shape with 8 sides would be a Octagon.\n" << endl;
        break;
        case 9:
        cout << "\n\nA shape with 9 sides would be a Nonagon.\n" << endl;
        break;
        case 10:
        cout << "\n\nA shape with 10 sides would be a Decagon.\n" << endl;
        break;
        default:
        cout << "\n\nERROR: Sorry, number input was not within designated range.\n" << endl;
        break;
    }
                                                           
    return 0; 
}
