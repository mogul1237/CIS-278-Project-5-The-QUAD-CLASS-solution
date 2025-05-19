# CIS-278-Project-5-The-QUAD-CLASS-solution

Download Here: [CIS 278 Project 5 The QUAD CLASS solution](https://jarviscodinghub.com/assignment/cis-278-project-5-the-quad-class-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

You are to implement a Quad class, such that you have both a ‘header file’ and an ‘implementation file ’ (see Chapter 11). The header file, Quad.h, provides class declaration and identifies public and private class members. The implementation file provides definitions for all member and friend functions.

A Quad object represents a Quadratic expression of degree 2, that is: ax2 + bx + c
For this assignment, the coefficients a, b and c are restricted to integers.

Public functions:
Quad()
Effect: create a Quadratic with a,b and c set to 0

Quad(int value)
Effect: creates a Quadratic with a=0, b=0, c = value

Quad(int a, int b, int c)
Effect: creates a Quadratic with the specified parameter values as coefficients

int eval(int value) const
Effect: evaluates the Quadratic for x = value
Postcondition: the Quad is unchanged
Returns: the computed result
For example, if the Quad equation was: 2×2 + 2x + 1
And method eval was called with value = 2, eval would return 14 ( 2*22 + 2*2 + 1)

int& operator[](int index)
Effect: set/access method for the coefficient of xindex
Returns: the coefficient of xindex

const Quad Quad::operator+(const Quad& qu) const // member function
Effect: overloads the + operator for Quad objects
Postcondition: this object and qu are unchanged
Returns: a new Quad object which is termwise sum of this object and qu

bool Quad::operator== (const Quad& q) const //member function
Effect: Compare this Quad to another object p to see if they are equal
Postcondition: this Quad object is unchanged
Returns:
A return value of true indicates that p refers to a Quad object
the same value as this Quad object. False is returned otherwise.

const Quad multiple(int value) const //member function
Effect: new Quad object is created in which each coefficient is a multiple of this object
Postcondition: this object is not changed
Returns: new object where each coefficient is ‘value times’ the coefficient of this object
(ie. this object a=2, b=4, c=3, value=6; new object a = 12, b =24, c = 18)
const Quad operator-() const // unary minus member function
Effect: new Quad object created identical to this one except coefficients are negated
Postcondition: this Quad object is unchanged
Returns: the new object

const Quad operator++() // autopreincrement member function
Effect: new Quad object created identical to this one after data is incremented
Postcondition: this Quad object coeffiecient are incremented by one
Returns: the new object

const Quad operator++(int) // autopreincrement member function
Effect: new Quad object created identical to this one before data is incremented
Postcondition: this Quad object coeffiecient are incremented by one
Returns: the new object

friend ostream& operator<<(ostream& out, const Quad& obj) //friend function Effect: outputs a string representation of this Quad Postcondition: this Quad object is unchanged Returns: a string of the form: a x2 + b x + c where a, b and c are the actual coeffients of the Quad object Quad operator-(const Quad& qu1, const Quad& qu2) //non- friend, non-member function Effect: overloads the binary - operator for Quad objects Postcondition: qu1 and qu2 are unchanged Returns: a new Quad object which is termwise difference of this qu1 and qu2 Application Contains a function void coefIn(int& value) which prompts for and reads an integer into a string object. This function verifies that all characters in the string are digits, and converts the digits to its integer representation. The function continues to reprompt the user until a valid string is provided. The integer is returned via the parameter list. You are to write an application (main program) which: • asks the user for coefficients a,b and c (use function coefIn(int& value)) • creates a Quad object, and outputs it to the screen • performs a variety of operations on this Quad object (and/or others created from it) such that all the correct operation of all is demonstrated. Be sure to provide output which clearly provides the result of each function call so that results can be verified. • test your functions in different scenerios – for example, statements such as q4 = (q1 - 2) + (q3 + q2); cout << "q4 is " << -q4 << endl; q5 = -(q1 + q2 + 2 - q3); cout << q5 << endl; where q1,q2,q3,q4 and q5 are Quad object, should work correctly. Submit files Quad.h, Quad.cpp, and your application.cpp file. Be sure that your name is included in each file and that all code is readable. Be sure to test your class thoroughly, as I will test it with applications other than your own.
