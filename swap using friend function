#include <iostream>
using namespace std;

class NumSwap {
private:
    int n1;
    int n2;

public:
    NumSwap(int a, int b) : n1(a), n2(b) {}

    // Declaration of friend function
    friend void swapNumbers(NumSwap &ns);
    
    void displayNumbers() {
        cout << "Num1: " << n1 << endl;
        cout << "Num2: " << n2 << endl;
    }
};

// Definition of the friend function
void swapNumbers(NumSwap &ns) {
    int temp = ns.n1;
    ns.n1 = ns.n2;
    ns.n2 = temp;
}

int main() {
    NumSwap ns(5, 10);
    cout << "Before swapping: " << endl;
    ns.displayNumbers();

    swapNumbers(ns);

    cout << "After swapping: " << endl;
    ns.displayNumbers();

    return 0;
}
