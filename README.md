# Assignment-submission-day3

Write a C++ program that contains a function called reverseString which takes a string as input and reverses it. The program should also include a main function that prompts the user to enter a string, calls the reverseString function to reverse the string, and then displays the reversed string.

#include <iostream>
#include <string>

using namespace std;

// Function to reverse a string
string reverseString(string str) {
  int n = str.length();
  for (int i = 0; i < n / 2; i++) {
    char temp = str[i];
    str[i] = str[n - 1 - i];
    str[n - 1 - i] = temp;
  }
  return str;
}

int main() {
  string str;
  cout << "Enter a string: ";
  getline(cin, str);

  // Reverse the string
  str = reverseString(str);

  // Print the reversed string
  cout << "The reversed string is: " << str << endl;

  return 0;
}
