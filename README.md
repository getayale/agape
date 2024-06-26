# agape

//c++ program that generate  fibonnaci  sequence by entering the number of terms


#include <iostream>

using namespace std;

int fibonacci(int n) {
    if (n <= 1)
        return n;
    
    return fibonacci(n - 1) + fibonacci(n - 2);
}

int main() {
    int num;

    cout << "Enter the number of terms in the Fibonacci sequence: ";
    cin >> num;

    cout << "Fibonacci Sequence: ";
    for (int i = 0; i < num; i++) {
        cout << fibonacci(i) << " ";
    }
    
    cout << endl;

    return 0;
}



