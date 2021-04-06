
.. contents::
   :local:
   :depth: 3
   
Bit Manipulation Algorithms
===============================================================================

Binary Number System
--------------------

in decimal 

.. image:: https://github.com/Love4684/practice/blob/main/media/1.jpg

in octal

.. image:: https://github.com/Love4684/practice/blob/main/media/2.jpg

in hexadecimal

.. image:: https://github.com/Love4684/practice/blob/main/media/3.jpg

in binary

.. image:: https://github.com/Love4684/practice/blob/main/media/4.jpg

 
Conversion 
--------------------

   * Decimal to Binary: Performing Division by Two with Remainder (For integer part)
   
   
   Ex 1.  Converting decimal number 112 into binary number.
   

      +------------------+------------------+
      |      Division    |   Remainder (R)  |
      +==================+==================+
      |    112 / 2 = 56	 |  0               |
      +------------------+------------------+
      |     56 / 2 = 28	 |  0               |
      +------------------+------------------+
      |     28 / 2 = 14	 |  0               |
      +------------------+------------------+
      |      14 / 2 = 7	 |  0               |
      +------------------+------------------+
      |       7 / 2 = 3	 |  1               |
      +------------------+------------------+
      |       3 / 2 = 1	 |  1               |
      +------------------+------------------+
      |       1 / 2 = 0	 |  1               |
      +------------------+------------------+
      
Now, write remainder from bottom to up (in reverse order), this will be
1110000 which is equivalent binary number of decimal integer 112.

   * Ex 2. Convert decimal fractional number 0.8125 into binary number.
 

      +------------------+------------------+
      |  Multiplication  | Resultant integer|
      |                  |   part (R)       |
      +==================+==================+
      |0.81252 x 2=1.625 |  1               |
      +------------------+------------------+
      | 0.6252 x 2= 1.25 |  1               |
      +------------------+------------------+
      |  0.252 x 2= 0.50 |  0               |
      +------------------+------------------+
      |    0.52 x 2= 1.0 |  1               |
      +------------------+------------------+
      |        0 x 2 = 0 |  0               |
      +------------------+------------------+
      
      
Now, write these resultant integer part, this will be 0.11010 which is equivalent binary fractional number of decimal fractional 0.8125.

Subtraction of two Binary Numbers(2 - 3)
--------------------

.. image:: https://github.com/Love4684/practice/blob/main/media/5.png

Bitwise Complement Operator
--------------------

It is important to note that the bitwise complement of any integer N is equal to -(N + 1). For example,

Consider an integer 35. As per the rule, the bitwise complement of 35 should be -(35 + 1) = -36.

.. image:: https://github.com/Love4684/practice/blob/main/media/6.webp

.. code:: c++

      #include <iostream>

      int main() {
          int num1 = 35;
          int num2 = -150;
          cout << "~(" << num1 << ") = " << (~num1) << endl;
          cout << "~(" << num2 << ") = " << (~num2) << endl;

          return 0;
      }
      
Output

~(35) = -36
~(-150) = 149
