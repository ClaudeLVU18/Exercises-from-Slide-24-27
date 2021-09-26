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
  
// Prev exercises(not sure if required but here to be safe)
  
//Print Biography 
#include <string> // allows string to be used
#include <stdlib.h>  

 int main()
{   
   cout << "\n\nPRINTING NAME, HOMETOWN, AND AGE.\n\n";
   
   string myName = Christian Claude L.V. Utlang
   string homeTown = Quezon City
   int age = 18
   cout << "\n\nHi I am " << myName << "\n\nI am from my hometown of " << homeTown << " which is located in the Philippines." << "\n\nAs of July 18th, I am now " << age << ".\n"; 
    cin.get();
    return 0; 
}
  
 //Print Biography with user input
#include <string> // allows string to be used
#include <stdlib.h>  

 int main()
{   
   cout << "\n\nINPUT NAME, HOMETOWN, AND AGE.\n\n";
    cout << "\n\nHi, what is your name? ";
    string myName;
    cin >> myName;

    cout << "\n\nOh, where are you from? ";
    string homeTown;
    cin >> homeTown;

    cout << "\n\nNice, how old are you now? ";
    int age;
    cin >> age;
    
    system("CLS");
    cout << "\n\nHi " << myName << "\n\nI see you are from " << homeTown << "." << "\n\nAnd that you are now " << age;
    cin.get();
    return 0; 
}
  
  
 //Convert Fahrenheit to Celsius  
#include <string> // allows string to be used
#include <stdlib.h>  

 int main()
{   
   cout << "\n\nCONVERTING FAHRENHEIT TO CELSIUS.\n\n";
    cout << "Hi, you can convert Fahrenheit to Celsius degrees here\n\n" << "Type in temperature in Fahrenheit: ";
    double fahrenheit;
    cin >> fahrenheit;
    double celsius = (fahrenheit - 32)*0.5556;
     
    cout << "\n\nThat would be " << celsius << " degrees celsius.\n\n";
    cin.get();
    return 0; 
}
  
 //Convert Celsius to Fahrenheit 
#include <string> // allows string to be used
#include <stdlib.h>  

 int main()
{   
   cout << "\n\nCONVERTING CELSIUS TO FAHRENHEIT.\n\n";
    cout << "Hi, you can convert Celsius to Fahrenheit degrees here\n\n" << "Type in temperature in Fahrenheit: ";
    double celsius;
    cin >> celsius;
    double fahrenheit = celsius*1.8 + 32;
     
    cout << "\n\nThat would be " << fahrenheit << " degrees fahrenheit.\n\n";
    cin.get();
    return 0; 
}
  
 //Print Biography 
#include <string> // allows string to be used
#include <stdlib.h>  

 int main()
{   
    cout << "\n\nF I N D I N G  A R E A  A N D  C I R C U M F E R E N C E  U S I N G  R A D I U S.\n\n";
    
    cout << "Enter radius of circle: \n";
    double rad;
    cin >> rad;
    double radsq = rad*rad;
    double pi = 3.14;
    double area = pi*radsq;
    double circ = pi*2*rad;
    cout << "\nThe area is: " << area << "\n\nThe circumference is: " << circ << "\n\n" <<endl;
    cin.get();
    return 0; 
}
  
 //Area for Rectangle, Square, Triangle 
#include <string> // allows string to be used
#include <stdlib.h>  

 int main()
{   
    system("CLS");
    cout << "\nArea finder for square, triangle, and rectangle.\n"; 
    cout << "\nChoose a shape to find the area for: ";
    cout << "\n\n1. Rectangle\n2. Triangle\n3.Square";
    cout<<"\n\nPlease select one and input its designated number (1, 2, or 3).\n" << endl;
    int shp;
    cin >> shp;

    switch(shp)
    {
        case 1:
            cout << "\n\nPlease enter the rectangle's length: ";
            double l;
            cin >> l;
            cout << "\n\nPlease enter the rectangle's width: ";
            double w;
            cin >> w;
            cout << "\n\nThe area of the rectangle is " << l*w;
            break;
         case 2:
            cout << "\n\nPlease enter the triangle's base: ";
            double b;
            cin >> b;
            cout << "\n\nPlease enter the rectangle's height: ";
            double h;
            cin >> h;
            cout << "\n\nThe area of the rectangle is " << b*h / 2;
            break;
        case 3:
            cout << "\n\nPlease enter the square's sides' length: ";
            double a;
            cin >> a;
            cout << "\n\nThe area of the rectangle is " << a*a;
            break;
        
        default:
            break;

    }


    return 0; 
}
  


