# CPP-Program-to-find-Permutations-in-which-n-people-can-occupy-r-seats-in-a-classroom

Which n people can occupy r seats in a classroom in C++
This is a problem specific program which deals with problems like in how many ways employees can be arranged in the seats available in a company or the same for the students in a school or college.

This problem can be easily solved by the use of the simple formula of permutations which is

Formula  =  n P r  =  n! / (n-r)!
Permutation
Way 2 Of Asking Question
Write code to find all possible permutations in which n people can occupy r seats in a theater
Problem Statement :
In a classroom some of the seats are already occupied by students and only a few seats are available in the classroom. The available seats are assumed as r and n number of students are looking for the seat. We need to find in how many different permutations n number of students can sit on r number of chairs.

Algorithm
Input number of students in n
Input number of seats in r
Use permutation formula { factorial(n) / factorial(n-r) }
Print Output
Permutations in which n people can occupy r seats in a class room
Related Pages
Octal to Binary conversion

Quadrants in which a given coordinate lies
 
Maximum number of handshakes

Addition of two fractions

Replace all 0’s with 1 in a given integer

While loop in C
C++ code
Run
//Permutations in which n people can occupy r seats
#include<iostream>
using namespace std;
    
//function for factorial
int factorial(int num)
{
    int fact=1;
    for(int i=num; i>=1 ;i--)
        fact*=i;
    return fact;
}
    
//main program
int main()
{
    int n,r;
    
    cout<<"Enter number of people: ";
    //user input
    cin>>n;
    
    cout<<"Enter number of seats: ";
    //user input
    cin>>r;
        
        
    //finding all possible arrangements of n people on r seats
    // by using formula of permutation
    int p = factorial(n)/factorial(n-r);

    //printing output
    printf("Total possible arrangements: %d",p);

    return 0;
}
Output
Enter number of people: 5
Enter number of seats: 9
Total possible arrangements: 120
