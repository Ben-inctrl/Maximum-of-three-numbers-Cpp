# Maximum-of-three-numbers-Cpp
A program that accepts three numbers and returns the maximum of the three.

#include <iostream>
using namespace std;

int numMax(int num, int num1, int num2);

int main(){
    int num, num1, num2;
    cout<<"Enter 3 numbers:\n";
    cin>>num>>num1>>num2;
    cout<<"The maximum number is:"<<numMax(num,num1,num2);
    return 0;
}

int numMax(int num, int num1, int num2){
    if((num>num1)&&(num>num2))
        return num;
    if((num1>num)&&(num1>num2))
        return num1;
    if((num2>num)&&(num2>num1))
     return num2;  
}


