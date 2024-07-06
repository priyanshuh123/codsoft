
#include <iostream>
#include <cstdlib>
#include <ctime>

using namespace std;

int main()
{

  srand((unsigned int) time(NULL));
  

  int number = (rand() % 100) + 1; 
  

  int guess = 0;
  
  do
  {
    // Prompt the user to enter the guess, store it into guess
    cout << "Enter Guess (1-100): ";
    cin >> guess;
    
    // Tell the user to guess higher or lower or that they won based on 
    // comparing the guess to the number.
    if (guess > number)
      cout << "Guess lower!" << endl;
    else if (guess < number)
      cout << "Guess higher!" << endl;
    else
      cout << "You won!" << endl;
      
    // Keep the game going by having the user guess again so long as they did 
    // not gue
  } while (guess != number);
   
  return 0;
}


