# Lecture-15-part-2

    #include <iostream>
    using namespace std;

    void myCalculation(int num) {
        num *= 2;
        num += 8;
        cout << num << endl;
     }
    int main()
    {
        int userNum;
        cout << "Enter A Number : ";
        cin >> userNum;
        myCalculation(userNum);

        return 0;
    }

Returning values

    #include <iostream>
    using namespace std;

    int myCalculation(int num) {
        num *= 2;
        num += 8;
        return num;
    }
    int main()
    {
        int userNum;
        cout << "Enter A Number: ";
        cin >> userNum;
        userNum = myCalculation(userNum);
        cout << userNum << endl;
        return 0;
    }
    
Purchase Products

    #include <iostream>
    using namespace std;

    /*
    double sumItems(double item1, double item2) {
        double total = item1 + item2;
        return total;
    }
    int main()
    {
        double myMoney = 40.00;
        double shoes = 25.99;
        double tshirt = 11.50;

        if (sumItems(shoes, tshirt) <= myMoney) {
             cout << "you can afford these items" << endl;
        }else{
            cout << "keep saving up" << endl;

        }
    }
    */

    double sumItems(double item1, double item2) {
        double total = item1 + item2;
        return total;
    }

    int main() {

        double myMoney = 40.00;
        double shoes{};
        double tshirt{};

        cout << "Enter the price for the shoes: ";
        cin >> shoes;
        cout << "Enter the price for the tshirt: ";
        cin >> tshirt;

        if (sumItems(shoes, tshirt) <= myMoney) {
            cout << "You can afford these items" << endl;
        }
        else {
            cout << "Better to just save up";
        }

    }

Time 

    #include <iostream>
    using namespace std;

    /*
    double sumItems(double item1, double item2) {
        double total = item1 + item2;
        return total;
    }
    int main()
    {
        double myMoney = 40.00;
        double shoes = 25.99;
        double tshirt = 11.50;

        if (sumItems(shoes, tshirt) <= myMoney) {
             cout << "you can afford these items" << endl;
        }else{
            cout << "keep saving up" << endl;

        }
    }
    */

    double sumItems(double item1, double item2) {
        double total = item1 + item2;
        return total;
    }

    int main() {

        double myMoney = 40.00;
        double shoes{};
        double tshirt{};

        cout << "Enter the price for the shoes: ";
        cin >> shoes;
        cout << "Enter the price for the tshirt: ";
        cin >> tshirt;

        if (sumItems(shoes, tshirt) <= myMoney) {
            cout << "You can afford these items" << endl;
        }
        else {
            cout << "Better to just save up";
        }

    }
    
Function time 

    #include <iostream>  
    using namespace std;
    /* return type set to string as this function will return a string value back  to main program */

    string greetings(int time) {
        //evaluate int value passed in and set return message 
        if (time < 12) {
            return "Good Morning";
        }
        else if (time >= 12 && time <= 17) {
            return "Good Afternoon";
        }
        else if (time >= 18 && time <= 21) {
            return "Good Evening";

        }
        else if (time >= 22 && time <= 24) {
            return "Good Night";
        }

    }
    int main() {
        cout << "What time is it? Enter the time in 24 format" << endl; //ask the user for time 
        int userInput; //variable to store user response
        cin >> userInput; //get user input

        //output string returned by function 
        cout << greetings(userInput) << endl;
        return 0;
    }
