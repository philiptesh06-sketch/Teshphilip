#include <iostream>
#include <string>
using namespace std;

class Employee {
private:
    string name;
    int age;
    int serviceYear;
    double salary;

public:
    // Parameterized constructor
    Employee(string n, int a, int sY, double sal) 
        : name(n), age(a), serviceYear(sY), salary(sal) {}

    // Destructor
    ~Employee() {
        cout << "Employee object destroyed." << endl;
    }

    // Accessor member functions
    string getName() { return name; }
    int getAge() { return age; }
    int getServiceYear() { return serviceYear; }
    double getSalary() { return salary; }
};

