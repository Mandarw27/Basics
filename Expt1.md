# AIM:
To learn about VS code and getting input from user and displaying it.

# Software Used
VS Code

# Problem Statement
1.) Write a program to print simple 'Hello world' message.

2.) Write a program to get the input from user and displaying it.

3.) Write a program to create a basic calculator.

# Theory
To print a message or output we use 'cout' .

The namespace is used to decrease or limit the scope of any variable or function.

'endl' is used to move the cursor to the new line.
```javascript
// Mandar Wankhede
// 23070123083
// Entc B1
//Experiment 1-Downloading and Installing VS Code, (Hello World and Calculator program)

#include <iostream>
using namespace std;
int main()
{
string a;

    
    cout<<"Enter your name  ";
    getline(cin,a);
    cout<<"Hello "<<a;
    return 0;
} 
```
<img width="339" alt="Screenshot 2024-08-23 at 10 14 39" src="https://github.com/user-attachments/assets/2014bc0a-8783-4483-8099-6a16a78275a8">

```javascript
#include<iostream>
using namespace std;
int main(){
    
    int a,b,c,d;
    cout<<"Calculator:1.Addition,2.subtraction,3.multiplication,4.division";
    cout<<"chose the operation you want to carry out";
    cin>>c;
    switch(c){
        case 1:
        {
         cout<<"Enter the first number:";
         cin>>a;
         cout<<"enter the second number:";
         cin>>b;
         d=a+b;
         cout<<d<<" is the sub of a and b";
         break;
        }
        case 2:
        {
         cout<<"Enter the first number:";
         cin>>a;
         cout<<"enter the second number:";
         cin>>b;
         d=a-b;
         cout<<d<<" is the subtraction of a and b";
         break;
        }
        case 3:
        {
         cout<<"Enter the first number:";
         cin>>a;
         cout<<"enter the second number:";
         cin>>b;
         d=a*b;
         cout<<d<<" is the product of a and b";
         break;
        }
        case 4:
        {
         cout<<"Enter the first number:";
         cin>>a;
         cout<<"enter the second number:";
         cin>>b;
         d=a/b;
         if(b==0)
        {
            cout<<"Invalid";
        }
         else
         {
         cout<<d<<" is the quotient";
         }
        }
     }

    

```
}<img width="749" alt="Screenshot 2024-08-23 at 10 17 45" src="https://github.com/user-attachments/assets/a7de35e4-75ed-4d20-a8a0-cb31de6b3e74">

<img width="764" alt="Screenshot 2024-08-23 at 10 19 11" src="https://github.com/user-attachments/assets/91411c35-d15b-4852-8345-448b1ae682b3">

<img width="764" alt="Screenshot 2024-08-23 at 10 19 52" src="https://github.com/user-attachments/assets/dcda07cc-4310-4e5c-a6d5-f918544a00ce">

<img width="764" alt="Screenshot 2024-08-23 at 10 25 16" src="https://github.com/user-attachments/assets/d55d1583-014c-483b-847f-d987491f0b67">
