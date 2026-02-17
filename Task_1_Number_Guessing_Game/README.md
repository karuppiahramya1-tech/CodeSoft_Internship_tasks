Task 1: Number Guessing Game

#include<iostream>
#include<cstdlib>
#include<ctime>
using namespace std;
int main(){
    srand(time(0));
    int n=rand()%100+1;
    while(1){
        int num;
        cout<<"Enter your guess:";
        cin>>num;
        if(num==n){
            cout<<"Your guess is correct"<<endl;
            break;
        }
        else if(num>n){
            cout<<"Too high try again"<<endl;
        }
        else if(num<n){
            cout<<"Too Low try again"<<endl;
        }
    }
}
