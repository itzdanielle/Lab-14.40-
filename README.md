# Lab-14.40-
#include <iostream>
using namespace std;

int main() {
  const int SECRET_NUMBER = 81;
  double number;
  int tries = 1;
   do { 
      cout << "Try to guess the secret number." << endl;
      cout << "Enter a number between 0 and 100." << endl;
      cin >> number;
    if (number < SECRET_NUMBER) 
      cout << "The number inputted is less than the secret number." << endl;
  
    else if (number < SECRET_NUMBER) 
      cout << "The number inputted is greater than the secret number." << endl;
  
    else if (number == SECRET_NUMBER) {
      cout << "You guessed it, you picked the secret number!" << endl;
      cout << "Number of tries " << tries << endl; 
      }
    else if ((number > 100) || (number < 0))
      cout << "Error: number must be between 0 and 100." << endl;
      tries++;
      
  }
  while (number != SECRET_NUMBER);




}
