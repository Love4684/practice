
.. contents::
   :local:
   :depth: 3
   
C++ OOPs Concepts
.........

oops is about creating objects that contain both data and functions.

Object
------------

Any entity that has state and behavior is known as an object. For example: chair, pen, table, keyboard, bike etc. It can be physical and logical.

Class
.........

A class is like a blueprint for an object. It is a user-defined data type, which holds its own data members and member functions.

Inheritance
------------

===============================================================================
When one object acquires all the properties and behaviours of parent object i.e. known as inheritance. It provides code reusability. It is used to achieve runtime polymorphism.

Polymorphism
------------

When one task is performed by different ways i.e. known as polymorphism. For example: to convince the customer differently, to draw something e.g. shape or rectangle etc.

In C++, we use Function overloading and Function overriding to achieve polymorphism.

Abstraction
------------

Hiding internal details and showing functionality is known as abstraction. For example: phone call, we don't know the internal processing.

In C++, we use abstract class and interface to achieve abstraction.

Encapsulation
------------

Binding code and data together into a single unit is known as encapsulation. For example: capsule, it is wrapped with different medicines.

Advantage of OOPs
------------

OOPs makes development and maintenance easier.

OOPs provide data hiding whereas in Procedure-oriented programming language a global data can be accessed from anywhere.

Why we need OOPs in Programming language?
------------

1. Duplicate code is a Bad.

2. Code will always be changed.

So, above statement proves, OOPs is provides code reusability which reduce the duplication of code because once you have duplicate code, you have make changes everywhere which leads to performance. Code can be changed anytime or requirement of application changed anytime so when you want to make changes in your application, OOPs makes it easier.

Structure vs class in C++
------------

1) Members of a class are private by default and members of a struct are public by default.

2) Both can have constructors, methods, properties, fields, constants, enumerations, events, and event handlers. 

struct for plain-old-data structures without any class-like features;

class when you make use of features such as private or protected members, non-default constructors and operators, etc.

.. code:: c++

    class Test {
        int x; // x is private
    };
    int main()
    {
      Test t;
      t.x = 20; // compiler error because x is private
      getchar();
      return 0;
    }
    
.. code:: c++
    
    #include <stdio.h>

    struct Test {
        int x; // x is public
    };
    int main()
    {
      Test t;
      t.x = 20; // works fine because x is public
      getchar();
      return 0;
    }

C++ Access Specifiers
------------

In C++, there are three access specifiers:

public - members are accessible from outside the class

private - members cannot be accessed (or viewed) from outside the class

protected - members cannot be accessed from outside the class, however, they can be accessed in inherited classes.

Types of Class Member Functions in C++
------------
Member functions are the functions, which have their declaration inside the class definition. The definition of member functions can be inside or outside the definition of class.

.. code:: c++

      class Cube
      {
          public:
          int side;
          int getVolume();
      };

      // member function defined outside class definition using the scope resolution ::
      int Cube :: getVolume()
      {
          return side*side*side;
      }

      int main()
      {
          Cube C1;
          C1.side = 4;    // setting side value
          cout<< "Volume of cube C1 = "<< C1.getVolume();
      }
