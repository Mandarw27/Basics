# AIM
To learn the execution and use of if statements & switch in c++.

# software used
VS CODE

# PROBLEM STATEMENT
1. Write a c++ program to check if the year is a leap year.
2.Write a c++ program to validate the password.
3.Write a c++ program to print days of week.
4.Write a c++ program to make a simple calculator.
5.) Write a c++ program to evaluate grades.

# Theory
Use if to specify a block of code to be executed, if a specified condition is true.
Use else to specify a block of code to be executed, if the same condition is false.
Use else if to specify a new condition to test, if the first condition is false.
Use switch to specify many alternative blocks of code to be executed.
The switch statement in C++ is a flow control statement that is used to execute the different
blocks of statements based on the value of the given expression. We can create different c
ases for different values of the switch expression. We can specify any number of cases 
in the switch statement but the case value can only be of type int or char.

 # codes
 ```javascript
#include<iostream>
using namespace std;
int main()
{
string password;
cout<<"enter your password: ";
cin>> password;
if(password==" secret")
{
cout<< "access granted";
}
else
{

cout<<"access denied";
}
}
```
 <img width="225" alt="Screenshot 2024-08-31 at 17 31 42" src="https://github.com/user-attachments/assets/64954ee6-275d-47ae-a0af-b5272676fc06">

```javascript
#include <iostream>
using namespace std;
int main()
{
int score;
cout<<"enter your score: ";
cin>> score;
if(score>=90){
cout<< "Grade: A"<< endl;}
else if(score>=80){
cout<< "Grade: B"<< endl;}
else if(score>=70){
cout<< " Grade: C"<<endl;}
else{
cout<< "Grade: F"<<endl;
}
}
```

<img width="184" alt="Screenshot 2024-08-31 at 17 34 20" src="https://github.com/user-attachments/assets/20a510be-4237-4014-b576-f36e0d2eff93">

```javascript
#include<iostream>
using namespace std;
int main()
{
    float a,b,c ;

    int choice;
    cout << "Calculator"<<endl;
    cout << "1: Addition"<<endl;
    cout << "2: Subtraction"<<endl;
    cout << "3: Multiplication"<<endl;
    cout << "4: Division"<<endl;
    cout<<"Enter operation choice: ";
    cin>>choice;
switch(choice)
{
    case 1 :
    { float c;
    cout<<"Enter numbers: ";
    cin>>a>>b;
    c=a+b;
    cout<<"sum is = "<<c;
    } 
    break;
    case 2 :
    {
        float c;
    cout<<"Enter numbers: ";
    cin>>a>>b;
    c=a-b;
    cout<<"difference is = "<<c;
    }
    break;
case 3 :
{ float c;
    cout<<"Enter numbers: ";
    cin>>a>>b;
    c=a*b;
    cout<<"product is = "<<c;
}
break;
case 4 :

{ float c;
   cout<<"Enter numbers: ";
    cin>>a>>b;
    c=a/b;
    cout<<"quotient is = "<<c;
    }
    break ;
}
return 0;
}
```
<img width="303" alt="Screenshot 2024-08-31 at 17 35 40" src="https://github.com/user-attachments/assets/26a2d818-9fe9-4301-aff9-b98a98d95098">

```javascript
#include<iostream>
using namespace std;
int main(){
cout<<"Enter the number of the day in the week(1-7)";
int a;
cin>>a;
switch(a)
{
    case 1:
    cout<<"Monday";
    case 2:
    cout<<"tuesday";
    case 3:
    cout<<"Wednesday";
    case 4:
    cout<<"Thursday";
    case 5:
    cout<<"Friday";
    case 6:
    cout<<"Saturday";
    case 7:
    cout<<"Sunday";
}

}
```
<img width="327" alt="Screenshot 2024-08-31 at 17 36 27" src="https://github.com/user-attachments/assets/fba913a3-703e-4a7b-aeac-646fcfce6fdd">

```javascript
#include<iostream>
using namespace std;
int main()
{
    int y;
    char c;
    cout<<"Enter year to check: ";
    cin>>y;
    if ( y%4==0 && y%100!=0 || y%400==0 )
    { cout<<y<<" is a leap year";}
    else
    { cout<<y<<" is not a leap year";}
    return 0;
}
```
<img width="188" alt="Screenshot 2024-08-31 at 17 38 32" src="https://github.com/user-attachments/assets/9157719b-a1d5-405d-b90c-c07895505b97">
