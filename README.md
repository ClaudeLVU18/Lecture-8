# Lecture-6


SWITCH MONTH DAYS

#include <iostream>
#include <string>

using namespace std;

	int main()
{
  cin.clear();
    cout << "\n\nDay checker for each month!\n\n";
    cout << "\n\npick a month\n";
    cout << "\n1.January\n2.February\n3.March\n4.April" << endl;
    cout << "5.May\n6.June\n7.July\n8.August" << endl;
    cout << "9.September\n10.October\n11.November\n12.December\n" << endl;
    cout << "Month: ";
    int input;
    cin >> input;
    cout << "\n\n";

    switch(input)
    {
        case 1:
        cout << "January has 31 days.";
        break;
        case 2:
        cout << "February has 29 days or 28 days on a leap year.";
        break;
        case 3:
        cout << "March has 31 days.";
        break;
        case 4:
        cout << "April has 30 days.";
        case 5:
        cout << "May has 31 days.";
        case 6:
        cout << "June has 30 days.";
        case 7:
        cout << "July has 31 days.";
        case 8:
        cout << "August has 31 days.";
        case 9:
        cout << "September has 30 days.";
        case 10:
        cout << "October has 31 days.";
        case 11:
        cout << "November has 30 days.";
        case 12:
        cout << "December has 31 days.";
        break;
        
        default:
        cout << "Invalid Input";
    }

	return 0;


}
  
  
  EXE GAME (would you like to play again)
  
  #include <iostream>
#include <string>

using namespace std;

	int main()
{
  cout << "\nWould you like to play again?" << endl;
    cout << "\nInput:\n'Y' if yes\n'N' if no" << endl;
    char input;
    cin >> input;

    switch(input)
    {
        case 'Y':
        case 'y':
            cout << "\nRestarting game..." << endl;
            break;
        case 'N':
        case 'n':
            cout << "\nExiting game... ";
            break;
        default:
            cout << "\nERROR: invalid input";

    }

	return 0;


}
  
  
  FUEL ME UP


#include <iostream>
#include <string>

using namespace std;
  
  
void F2Ffuelmeup()
{
    cout << "\n\nHi, Welcome to ADNOC, select gas  you want\n\n";
    cout << "\n\nInput 'p' for petrol\nInput 'd' for diesel\n\n";
    char fuel;
    cin >> fuel;
    
    switch(fuel)
        {
        case 'p':
        case 'P':
            cout << "\nOk, how many litres?\n\n";
            cout << "L:";
            int la;
            cin >> la;
            cout << "\nThat would be $"<<2.44*la<<"\n" << endl;
            break;
            

        case 'd':
        case 'D':
            cout << "\n\nOk, how many litres?\n\n";
            cout << "\n\nL:";
            int lc;
            cin >> lc;
            cout << "\nThat would be $"<<2.38*lc<<"\n" << endl;
            break;
        default:
        {
            cout << "\nERROR: Please select between petrol or diesel.\n"<<endl;
            F2Ffuelmeup();

             
        }
        
           
        }
    

}
  
 
	int main()
{
  F2Ffuelmeup();

	return 0;


}
  
  
  
  SWITCH TEMPERATURE CONVERTER
  
  
#include <iostream>
#include <string>

using namespace std;
  
  void FahtoCel()
{
    cout << "\n\nCONVERTING FAHRENHEIT TO CELSIUS.\n\n";
    cout <<"Type in temperature in Fahrenheit: ";
    double fahrenheit;
    cin >> fahrenheit;
    while(cin.fail())
    {
        cout << "\nERROR: not a valid input.\nPlease re-enter temperature in Celsius: ";

        cin.clear();
        cin.ignore(1000, '\n');
        cin >> fahrenheit;

    }
    double celsius = (fahrenheit - 32)*0.5556;
     
    cout << "\n\nThat would be " << celsius << " degrees celsius.\n\n";
    cin.get();

}

void CeltoFah()
{
    cout << "\n\nCONVERTING CELSIUS TO FAHRENHEIT.\n\n";
    cout << "Type in temperature in Fahrenheit: ";
    double celsius;
    cin >> celsius;
    while(cin.fail())
    {
        cout << "\nERROR: not a valid input.\nPlease re-enter temperature in Fahrenheit.";

        cin.clear();
        cin.ignore(1000, '\n');
        cin >> celsius;

    }
    double fahrenheit = celsius*1.8 + 32;
     
    cout << "\n\nThat would be " << fahrenheit << " degrees fahrenheit.\n\n";
    cin.get();

}

    int main()
{
    system("CLS");

    cout << "\nCelsus and Fahrenheit Temperature converter\n\n";
    cout << "1. Celsius to Fahrenheit.\n2. Fahrenheit to Celsius.\n\n";
    cout << "Select a temperature type converter (1/2):  ";

    int userInput;
    cin >> userInput;

  

    switch (userInput)
    {
    case 1:
        CeltoFah();

        break;

    case 2:
        FahtoCel();

        break;
    
    default:

        
        
        cout << "ERROR: not a valid option.";
        
        
        
        
        break;
  
        return 0;
    }
}
  
  
  NAME THAT SHAPE

#include <iostream>
#include <string>

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


  CAPITAL OF FRANCE
  
  #include <iostream>
#include <string>

using namespace std;

	int main()
{
  cout << "What is the capital of France?\n";
    string capital;
    cin >> capital;

    if ((capital == "Paris")||(capital == "paris")||(capital == "PARIS"))
    {
        cout << "\nThat is correct.";
    }

	return 0;


}


  GRADE MARKS SWITCH
  
  
#include <iostream>
#include <string>

using namespace std;
  
 int main()
{
  cout << "Enter your full name" << endl;
    string stdntName;
    getline(cin, stdntName);
    

    cout << "\nEnter your grade marks (0-100):  ";


    int grade;

    cin >> grade;
    if (cin.fail())
    {
        cin.clear();
        cin.ignore();
        cout << "ERROR: not a valid input.";
    }

    else if (grade > 100)

    {


        cout << "\nPlease keep your marks within 0-100\n";
    }

    else

    {

        switch (grade/10)

        {

        case 10:

        case 9:
        case 8:

        {
            


            cout << stdntName <<", your grade is: A";


            break;
        }
        case 7:

        {    


            cout << stdntName << ", your grade is: B";


            break;
        }
        case 6:
        {
            


            cout << stdntName << ", your grade is: C";

            break;
        }
        case 5:
        {
            

            cout << stdntName << ", your grade is: D";


            break;
        }
        case 4:
        {
            



            cout << stdntName << ", your grade is: E";



            break;
        }
        default:
        {
            


            cout << stdntName << ", your grade is: F\n";


        }
        }
    }

	return 0;


}



