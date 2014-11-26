// Lab 4c, Tabular Formatting
// Programmer: Sohaib Syed
// Editor(s) used: CodeBlocks
// Compiler(s) used: CodeBlocks

#include <iostream>
using std::cin;
using std::cout;
using std::endl;

#include <cstdlib>

#include <ctime>

void interpret (int& num, int& userGuess);
void guess(int& num, int& userGuess);

int main()
{
  //Sohaib Syed, Tabular Formatting
  cout << "Lab 4c, Tabular Formatting \n";
  cout << "Programmer: Sohaib Syed\n";
  cout << "Editor(s) used: CodeBlocks\n";
  cout << "Compiler(s) used: CodeBlocks\n";
  cout << "File: " << __FILE__ << endl;
  cout << "Compiled: " << __DATE__ << " at " << __TIME__ << endl << endl;

  srand(time(0));
  int userGuess;
  int num;
  char answer;
  char buf[100];

  interpret(num, userGuess);
  guess(num, userGuess);
    do
    {
      cout << "Excellent! You guessed the number!\n";
      cout << "Would you like to try again (y or n)\n";
      cin >> buf;
      answer = buf[0];
      if(answer == 'Y' || answer == 'y')
      {
        interpret(num, userGuess);
        guess(num, userGuess);
      }
    }while(buf[0] == 'Y' || buf[0] == 'y');
       while(buf[0] == 'N' || buf[0] == 'n')break;
}

void interpret (int& num, int& userGuess)
{
  char buf[100];
  num = rand() % 1000 + 1;
  cout << endl;
  cout << "I have a number between 1 and 1000\n";
  cout << "Can you guess my number?\n";
  cout << "Please type your first guess: \n";
  cin >> buf;
  userGuess = atoi(buf);
}

void guess(int& num, int& userGuess)
{
  while(num != userGuess)
  {
    if(num > userGuess)
    {
      cout << "Too low. Try again." << endl;
      cin >> userGuess;
    }
    else if(num < userGuess)
    {
      cout << "Too high. Try again." << endl;
      cin >> userGuess;
    }
  }
}
