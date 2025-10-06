# Inheritance-
// Program-2
#include <iostream>
using namespace std;

int main() {
    int age;

    cout << "Enter age: ";
    cin >> age;

    try {
        if (age < 18) {
            throw age; // exception throw
        } else {
            cout << "Age: " << age << "\nAPPROVED" << endl;
        }
    }
    catch (int a) {
        cout << "\nERROR: Underage! (" << a << ")" << endl;
    }

    return 0;
}
