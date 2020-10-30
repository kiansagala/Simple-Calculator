# Simple-Calculator
# include <iostream>
using namespace std;

int main()
{
    int op;
    float num1, num2;

	cout <<	"[1]. Addition" << endl;
	cout <<	"[2]. Subtraction" << endl;
	cout <<	"[3]. Multiplication" << endl;
	cout <<	"[4]. Division" << endl;
	cout << "Choose operator: ";
    cin >> op;
    
    while (op > 4 || op <= 0)
    {
        cout << "Error! number should in range of (1 to 4)." << endl << endl;
        cout << "Enter the number again: ";
        cin >> op;
    }
 
    cout << endl << "Enter number: ";
    cin >> num1;
    cout << "Enter number: ";
    cin >> num2;

    switch(op) {
        case 1:
            cout << num1 << " + " << num2 << " = " << num1+num2;
            break;

        case 2:
            cout << num1 << " - " << num2 << " = " << num1-num2;
            break;

        case 3:
            cout << num1 << " * " << num2 << " = " << num1*num2;
            break;

        case 4:
        if (num2==0){
        	cout << num1 << " CANNOT DIVIDE BY 0";
        }
        else
            cout << num1 << " / " << num2 << " = " << num1/num2;
            break;

    }
    
	cout << endl <<"BY: KIAN SAGALA";
    return 0;
}

