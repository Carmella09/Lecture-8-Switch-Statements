# LEC-8-Codes

//SWITCH STATEMENT 

 Simple Calculator 

      #include <iostream>
    using namespace std;
    int main()
    {
        int a, b;
        cout << "Enter two numbers" << endl;
        cin >> a >> b;
        cout << "Pick a calculation" << endl;
        cout << "1: Addition\n2: Subtraction\n3: Multiplication\n4: Division" << endl;
        int input; 
        cin >> input;
          switch (input) {
          case 1:
              cout << (a + b);
              break;
          case 2:
              cout << (a - b) << endl;
              break;
          case 3: 
              cout << (a * b) << endl;
              break;
          case 4:
              cout << (a / b) << endl;
              break;
          default:
              cout << "Invalid Input\n";
          }
      }


  Grouping Cases

        #include <iostream>
      using namespace std;
      int main()
      {
          cout << "Would you like sugar?" << endl;
          char input;
          cin >> input;

          switch (input) {
          case 'Y':
          case 'y':
              cout << "Adding sugar..." << endl;
              break;
          case 'N':
          case 'n':
              cout << "No sugar requested..." << endl;
              break;
          default:
              cout << "That input was not recodgnised" << endl;

          }
      }

//EXERCISES

Continue? (Gameplay)

      #include <iostream>
    using namespace std;
    int main()
    {
        cout << "Would you like to continue? (Y/N): " << endl;
        char input;
        cin >> input;

        switch (input) {
        case 'Y':
        case 'y':
            cout << "Continuing the game" << endl;
            break;
        case 'N':
        case 'n':
            cout << "Going back to the main lobby" << endl;
            break;
        default:
            cout << "What? Please Try again" << endl;
            cin.get(); 
        }
    }



   Days in Months

    #include <iostream>
    using namespace std;
    int main()
    {
        cout << "Please enter the Month's number (e.g. 1 = Januray, 12 = December): " << endl;
        int input;
        cin >> input;

        switch (input) {
        case 1:
            cout << "31 Days" << endl;
            break;
        case 2:
            cout << "28 Days" << endl;
            break;
        case 3:
            cout << "31 Days" << endl;
            break;
        case 4:
            cout << "30 Days" << endl;
            break;
        case 5:
            cout << "31 Days" << endl;
            break;
        case 6:
            cout << "30 Days" << endl;
            break;
        case 7:
            cout << "31 Days" << endl;
            break;
        case 8:
            cout << "31 Days" << endl;
            break;
        case 9:
            cout << "30 Days" << endl;
            break;
        case 10:
            cout << "31 Days" << endl;
            break;
        case 11:
            cout << "30 Days" << endl;
            break;
        case 12:
            cout << "31 Days" << endl;
            break;
        default:
            cout << "What? Please Try again" << endl;

        }
    }


 
   Fuel me up (Face to Face Group)

      #include <iostream>
    using namespace std;
    int main()
    {
        int lit;
        cout << "How many liters of fuel do you need sir/maam?" << endl;
        cin >> lit;

        if (lit != 0)
        {
            cout << "Which type of fuel you would like to use? (P for Petrol/D for Diesel): ";
            char fuel;
            cin >> fuel;

            switch (fuel)
            {
            case 'p':
            case 'P':
            {
                cout << "You have chosen Petrol" << endl;
                double cp;

                cp = lit * 2.5;
                cout << "The price of your fuel is: " << cp << endl;
                break;
            }
            case 'D':
            case 'd':
            {
                cout << "You have chosen Diesel" << endl;
                double dp;

                dp = lit * 5;
                cout << "The price of your fuel is: " << dp << endl;
                break;

                break;
            }

            default:
            {
                cout << "Invalid input";
                break;
            }
        }
        }

        else {
            cout << "Invalid Input" << endl;
        }

    }


  Switching Temperature (Face to Face Group) version

      #include <iostream>
    using namespace std;

    int main()
    {
        double val;
        cout << "What is your temperature? Enter the value in numbers: ";
        cin >> val;
        char temp;

        if (val != 0)
        {
            cout << "What is your unit of temperature? C or F: " << endl;
            cin >> temp;
            double fahr = (val * 1.8) + 32;
            double cel = (val - 32) * 0.5556;

            switch (temp)
            {
            case 'f':
            case 'F':
                cout << "Your temperature in Celsius: " << cel << endl;

                break;

            case 'c':
            case 'C':
                cout << "Your temperature in Fahrenheit: " << fahr << endl;

                break;

            default:

                cout << "Invalid Input" << endl;
            }
        }
        else
            cout << "Invalid Input" << endl;
    }



Bonus Exercise: Switch Grade Calculator (The first code I made) version (1) 

    #include<iostream>
    #include<string>
    using namespace std;
    int main()
    {
        cout << "Student's name: " << endl;
        string name;
        cin >> name;

        cout << "Enter your Grade (between 0 - 100): " << endl;
        int grade;
        cin >> grade;

        {
            switch (grade / 10) {
            case 10:
            case 9:
            case 8:
                cout << "Your grade is A" << endl;
                break;
            case 7:
                cout << "Your grade is B" << endl;
                break;
            case 6:
                cout << "Your grade is C" << endl;
                break;
            case 5:
                cout << "Your grade is D" << endl;
                break;
            case 4:
                cout << "Your grade is E" << endl;
                break;
            case 3:
            case 2:
            case 1:
                cout << "Your grade is F" << endl;
                break;
            default:
                cout << "Invalid output" << endl;
                cout << "But if its 0, 1, 2, 3, 4, 5, 6, 7, 8, and 9 your grade is F" << endl;
            }
        }
    }
    
Bonus Exercise: Switch Grade Calculator (improved) version (2)

     #include<iostream>
     #include<string>
     using namespace std;
     int main()
     {
         cout << "Student's Full name: " << endl;
         string name;
         getline (cin, name);

         cout << "Enter your Grade (between 0 - 100): " << endl;
         int grade;
         cin >> grade;
         if (!cin.fail())
         
         {
             switch (grade / 10) {
             case 10:
             case 9:
             case 8:
                 cout << "Your grade is A" << endl;
                 break;
             case 7:
                 cout << "Your grade is B" << endl;
              break;
          case 6:
              cout << "Your grade is C" << endl;
              break;
          case 5:
              cout << "Your grade is D" << endl;
              break;
          case 4:
              cout << "Your grade is E" << endl;
              break;
          case 3:
          case 2:
          case 1:
          case 0:
              cout << "Your grade is F" << endl;
              break;
          default:
              cout << "Invalid output" << endl;
          }

      }

      else if(cin.fail())
      {
          cin.clear();
          cin.ignore(1000, '\n');
          cout << "Invalid output" << endl;

      }
  }
 

//SWITCH STATEMENT PART 2

   Switching Temperature (Online By myself) version (1)

      #include <iostream>
    using namespace std;
    int main()
    {
        double no;
        cout << "Please write the temperature: " << " " << endl;
        cin >> no;
        char temperature;
        cout << "Enter F to convert from Farenheit " << endl << "Enter C to convert from Celsius " << endl;
        cin >> temperature;

        switch (temperature) {
        case 'c':
        case 'C':
            cout << (no - 32) * 0.5556;
            break;
        case 'f':
        case 'F':
            cout << (no * 1.8) + 32;
            break;

        default:
            cout << "What? Please try again" << endl;
        }
    }


   Switching Temperature (Online By myself) version (2)

      #include <iostream>
    using namespace std;
    int main()
    {
        double no;
        cout << "Please write your temperature: " << " " << endl;
        cin >> no;
        char temperature;

        cout << "Enter F to convert from Farenheit " << endl << "Enter C to convert from Celsius " << endl;
        cin >> temperature;
        double celsius = (no - 32) * 0.5556;
        double farenheit = (no * 1.8) + 32;

        switch (temperature)
        {
        case 'c':
        case 'C':
            cout << "Celsius: " << celsius << endl;

            break;

        case 'f':
        case 'F':
            cout << "Fahrenheit: " << farenheit << endl;

            break;

        default:

            cout << "What? Please try again" << endl;
        }
    }


   Shape

      #include <iostream>
    using namespace std;
    int main()
    {
        int side;
        cout << "Enter the sides number to see the shape name (minimum 3 sides, maximum 10)" << endl;
        cin >> side;

        switch (side) {
        case 3:
            cout << "Triangle  has " << side << " sides" <<  endl;
            break;
        case 4:
            cout << "Sqaure/Rectangle  has " << side << " sides" << endl;
            break;
        case 5:
            cout << "Pentagon  has " << side << " sides" << endl;
            break;
        case 6:
            cout << "Hexagon   has " << side << " sides" << endl;
            break;
        case 7:
            cout << "Hepaton  has " << side << " sides" << endl;
            break;
        case 8:
            cout << "Octagon  has " << side << " sides" << endl;
            break;
        case 9:
            cout << "Nonagon  has " << side << " sides" << endl;
            break;
        case 10:
            cout << "Decagon  has " << side << " sides" << endl;
            break;
        default:
            cout << "What? Try again" << endl;
            break;
        }
    }


   France 

      #include <iostream>
    using namespace std;
    int main()
    {
        cout << "What is the capital of France?\n" << endl
             << "A. Tokyo" << endl << "B. Paris" << endl << "C. Bangkok" << endl << "D. Toronto\n" << endl;
        char capital;
        cin >> capital;

        switch (capital) {
        case 'b':
        case 'B': 
            cout << "You are Right!" << endl;
            break;
        case 'a':
        case 'A':
        case 'c':
        case 'C':
        case 'd':
        case 'D':
            cout << "You are wrong lol\n" << endl;
            break;
        default:
            cout << "What? Try again\n" << endl;
            break;
        }
    }

  
