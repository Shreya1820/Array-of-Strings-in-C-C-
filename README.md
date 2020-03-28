# Array-of-Strings-in-C/C++

Array of Strings in C++ (3 Different Ways to Create)
In C/C++, a string is a 1-D array of characters and an array of string in C is a 2D array of characters. This comes quite handy in C++. There are 3 ways in which an Array of Strings in C or C++ can be created.

Using 2D array(Both C and C++): This method is useful for shuffling, comparing and accessing characters randomly.
Syntax:
Char “Name” [“Number of Strings”][“MaxSize of String”]
Example:

Char colour [4][10]
// Here 4 colours can be inserted 
// with max String size of 10.


filter_none
edit
play_arrow

brightness_4
// C++ program to demonstrate array of strings using 
// 2D character array 
#include <bits/stdc++.h> 
using namespace std; 
  
int main() 
{ 
    // Initialize 2D array 
    char colour[4][10] = { "Blue", "Red", "Orange", 
                           "Yellow" }; 
  
    // Printing Strings stored in 2D array 
    for (int i = 0; i < 4; i++) 
        cout << colour[i] << "\n"; 
  
    return 0; 
} 
Output:
Blue
Red
Orange
Yellow
Drawbacks:

Both the number of Strings and Size of String are fixed.
A 2D array is allocated, whose second dimension is equal to maximum sized string which causes wastage of space.
Using string Keyword (Only in C++): In this method, size of the string is not fixed, hence space is saved.
Syntax:
String Name_ofString [number_of_string]
Example:

String geeks[50]
filter_none
edit
play_arrow

brightness_4
// C++ program to demonstrate array of strings using 
// array of strings. 
#include <bits/stdc++.h> 
using namespace std; 
  
int main() 
{ 
    // Initialize String Array 
    string colour[4] = { "Blue", "Red", 
                         "Orange", "Yellow" }; 
  
    // Print Strings 
    for (int i = 0; i < 4; i++) 
        cout << colour[i] << "\n"; 
} 
Output:
Blue
Red
Orange
Yellow
Drawback: The array is of fixed size.

Using Vectors(Only C++): STL Container Vector can be used to dynamically allocate array.
Syntax:

Vector “Name”
Example:

Vector Colour
filter_none
edit
play_arrow

brightness_4
// C++ program to demonstrate vector of strings using 
#include <bits/stdc++.h> 
using namespace std; 
  
int main() 
{ 
    // Declaring Vector of String type 
    vector<string> colour; 
  
    // Initialize vector with strings using push_back 
    // command 
    colour.push_back("Blue"); 
    colour.push_back("Red"); 
    colour.push_back("Orange"); 
    colour.push_back("Yellow"); 
  
    // Print Strings stored in Vector 
    for (int i = 0; i < colour.size(); i++) 
        cout << colour[i] << "\n"; 
} 
Output:
Blue
Red
Orange
Yellow
Conclusion: Out of all the three methods, Vector seems to be the best way for creating an array of Strings in C++.
