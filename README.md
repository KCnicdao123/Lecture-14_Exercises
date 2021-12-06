# Lecture-14_Exercises

//Exercise 1

#include <iostream>
#include <string>
#include <algorithm>
#include <array>
#include <random>
  
using namespace std; 
  
int main()
{
	int randomArray[1000], y = 0;
	srand(7);
	for (int x = 0; x < 1000; x++) {
		randomArray[x] = rand() % 50;
		cout << randomArray[x] << endl;
		if (randomArray[x] == 6) {
			y++;
		}
	}
	cout << "The number 6 appeared: " << y << " times." << endl;
}
--------------------------------------------
                                  
//Exercise 2
            
#include <iostream>
#include <string>
#include <algorithm>
#include <array>
#include <random>

using namespace std;
  
int main()
{
	array<int, 10> userInput;
	cout << "Enter 10 numbers and I will show you the largest number." << endl;
	for (int x = 0; x < 10; x++) {
		cin >> userInput[x];
	}
	reverse(userInput.begin(), userInput.end());
	cout << "\nThe largest number is: " << userInput[0];
}
-------------------------------------------------------------------------------------
//Exercise 3
  
#include <iostream>
#include <string>
#include <algorithm>
#include <exception>
#include <array>
#include <random>

using namespace std;
  
int main()
{
	array<int, 10> userInput;
	cout << "Enter 10 numbers and I will show you the largest number." << endl;
	for (int x = 0; x < 10; x++) {
		cin >> userInput[x];
	}
	sort(userInput.begin(), userInput.end());
	cout << "\nThe smallest number is: " << userInput[0];
}
