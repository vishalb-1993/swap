#include <iostream>
using namespace std;
class Number {
private:
    int value;

public:
    Number(int val) : value(val) {}

    // Overloading the + operator for number swapping
    Number operator+(const Number &other) {
        Number temp = *this;
        value = other.value;
        value = temp.value;
        return *this;
    }

    int getValue() const {
        return value;
    }
};

int main() {
    Number a(5);
    Number b(10);

    cout << "Before swapping: a = " << a.getValue() << ", b = " << b.getValue() << endl;

    // Swapping using operator overloading
    a = a + b;

    cout << "After swapping: a = " << a.getValue() << ", b = " << b.getValue() << endl;

    return 0;
}
