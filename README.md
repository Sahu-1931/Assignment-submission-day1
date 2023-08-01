# Assignment-submission-day2

Write a program in C++ that takes an input number from the user and determines whether it is even or odd. If the number is even, the program should display the message "Number is even." If the number is odd, the program should display the message "Number is odd."

#include <iostream>

using namespace std;

int main() {
  // Get the number from the user
  int number;
  cout << "Enter a number: ";
  cin >> number;

  // Check if the number is even
  if (number % 2 == 0) {
    cout << "Number is even." << endl;
  } else {
    cout << "Number is odd." << endl;
  }

  return 0;
}
