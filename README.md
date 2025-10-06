CODE 1
1.Start program.

2.Define class Vehicle:

public data member brand initialized to "Ford".

public member function color() that writes "red" to standard output.

3.Define class car that publicly inherits Vehicle:

public data member model initialized to " Mustang" (note the leading space).

In main():

4.Create an object c of type car. This object contains brand and model.

Call c.color(). This prints the string "red" to the console (no newline).

Evaluate c.brand + " " + c.model to produce a single std::string and send it to cout.

5.Return 0 and exit program.
Start program.

CODE 2:
Define class Vehicle:

public member company initialized to "FORD".

public method type() that prints Mustang followed by a newline.

Define class Specs:

public member mileage initialized to "8 kmpl".

public method color() that prints Grey followed by a newline.

Define class Car that publicly inherits from both Vehicle and Specs:

public member seater initialized to "4 seater".

In main():

Construct an object f2 of type Car.

Call f2.color() → runs Specs::color() and prints Grey + newline.

Output f2.company followed by a single space (no newline).

Call f2.type() → runs Vehicle::type() and prints Mustang + newline.

Output (, then f2.seater, then ) and a newline.

Output the literal "mileage:" immediately followed by f2.mileage and a newline.

Return 0 (program exits).

Line-by-line mapping (what each key line does)

Car f2; → constructs f2 with company="FORD", mileage="8 kmpl", seater="4 seater".

f2.color(); → prints Grey and newline.

cout << f2.company << " "; → prints FORD and a single space (no newline).

f2.type(); → prints Mustang and newline (so line becomes FORD Mustang).

cout << "(" << f2.seater << ")" << endl << "mileage:" << f2.mileage << endl;

prints (4 seater) then newline,

prints mileage:8 kmpl then newline.

Program output (exact lines)
Grey
FORD Mustang
(4 seater)
mileage:8 kmpl

Program-4: Hierarchical Inheritance
This program demonstrates the concept of hierarchical inheritance combined with multilevel inheritance (hybrid inheritance) in C++. The base class Entc contains the total number of students. From this class, two branches are created: Vlsi and Embedded, each representing specialized domains. Further, Verifengg and Designengg are derived from Vlsi, while Developer and Micro are derived from Embedded. This structure creates a tree-like hierarchy where multiple classes share common properties from a single base class. In the main() function, objects of different derived classes are created, and student data is assigned for each specialization. This illustrates how hybrid inheritance allows organizing data across multiple related categories while reusing the base class attributes.

--> Algorithm:
1.Start the program.

2.Define a base class Entc with a data member students to store total students.

3.Define two derived classes from Entc: --Vlsi for VLSI department. --Embedded for Embedded Systems department.

4.Define further derived classes: --From Vlsi: Verifengg (Verification Engineers) and Designengg (Design Engineers). --rom Embedded: Developer (Developers) and Micro (Microcontroller students).

5 In the main() function: --Create objects of Verifengg, Designengg, Developer, and Micro. --Assign values to students and specialization-specific data members.

6.End the program.

Program-5: Access Specifiers
This program demonstrates the use of access specifiers and protected inheritance in C++. The base class Github has members with public, private, and protected access levels. The class User inherits from Github using protected inheritance, which means that the public and protected members of Github become protected in User. In the main() function, the program tries to access private and protected members, which is not allowed outside the class, leading to access errors. This illustrates how access specifiers control visibility and accessibility of class members in inheritance, ensuring data encapsulation and security of sensitive information.

--> Algorithm:
1.Start the program.

2..Define a base class Github with: --A public function disp(). --A private function disp2(). --A protected data member repo.

3.Define a derived class User that inherits protectedly from Github. --Add a public data member user_id. In the main() function: --Create an object g1 of Github and try to call disp2() (will cause an error because it is private). --Create an object u1 of User. --Assign a value to user_id. --Try to access disp() and repo (access errors occur because of protected inheritance).

4.End the program.
