# Number-Guessing-Game
This is a number guessing game
#include<iostream>
using namespace std;
// This is a number guessing game
int main(){
    int num;
    int guess;
    int tries;
    srand(time(NULL));
    num = (rand() %100) +1; 
    cout << "Welcome Player!\n";
   do{ 
       
       cout << " Please enter a random number between 1-100\n";
       cin >> guess;
       tries++;
       
       if(guess > num){
           cout << " Too High\n ";
       }
       else if(guess < num){
           cout << " Too Low\n ";
       }
       else{
           cout << " You Got it!!! tries:" << tries << '\n';
       }
        
        
    }while(guess != num);
    
    
  return 0;
    
}
