
# AIM
To learn about costructor and destroctor in c++.

# Software Used
online compiler

# Problem Statement
1.) Write a c++ program to define constructor.

2.) Write a c++ program using parameterized constructior.

3.) Write a c++ program using copy constructor.

4.) Write a c++ program for default argument.

5.) Write a c++ program to calculate area of rectangle using class.

6.) Write a c++ program using deconstructor.

# Theory
Constructor: A constructor is a member function of a class that has the same name as the class name. It helps to initialize the object of a class
It can either accept the arguments or not. It is used to allocate the memory to an object of the class. It is called whenever an instance of the class is created. 
It can be defined manually with arguments or without arguments. There can be many constructors in a class. It can be overloaded but it can not be inherited or virtual.

# codes:
~~~//DEFINE CONSTRUCTOR.
#include<iostream>
using namespace std;
class MyClass{
    public:
    string a;
MyClass(){

    cout<< "Enter your name: "<<endl;
    cin>>a;
    cout<<"Hello "<<a<< " from constructor !!"<<endl;

}
};
int main(){
    MyClass obj;
    return 0;
}
~~~
//output:
<img width="220" alt="Screenshot 2024-10-15 at 12 10 18 PM" src="https://github.com/user-attachments/assets/bf8bef95-b352-4408-ad6b-b81fa93da62b">


~~~//PARAMETERIZED CONSTRUCTOR
#include<iostream>
using namespace std;
class MyClass{
    public:
    int c;
    MyClass(int val)
{
    c = val*val;
    cout<<"Square of "<<val<<" is: "<<c<<endl;
    
}
};
int main() {
    MyClass obj(5);
    return 0;
}
~~~
//output:
<img width="211" alt="Screenshot 2024-10-15 at 12 12 03 PM" src="https://github.com/user-attachments/assets/22ffae2e-dcc6-4c81-9e99-8aa2cf500266">


~~~//COPY CONSTRUCTOR
#include<iostream>
using namespace std;
class MyClass{
    private:
    int value;
    public:
    MyClass(int val){
        value = val;
        cout << "Build "<<value<<endl;

    }
    MyClass(const MyClass &obj){
        value = obj.value;
        cout<<" Create Blog "<<value<<endl;
    }
};
int main(){
    MyClass obj1(2024);
    MyClass obj2 = obj1 ;
    return 0;
    }

~~~

// output: 
<img width="216" alt="Screenshot 2024-10-15 at 12 14 21 PM" src="https://github.com/user-attachments/assets/88c75cc7-919f-41f7-b243-ce370809de01">



~~~//DEFAULT ARGUMENT
#include<iostream>
using namespace std;
class MyClass{
    private:
    int value1;
    int value2;
    string str1;
    public:
    
    MyClass( int val1= 0, int val2= 0, string a = "none"){
        str1 = a;
        value1= val1;
        value2 = val2;
        cout<<str1<<" played "<<value1<<"  matches."<<endl;
        cout<<"He scored "<< value2 << " goals."<<endl;

    }
};
int main()
{
   
    MyClass obj1(1900,900, "Ronaldo");
    return 0;
    }
~~~
//output:
<img width="220" alt="Screenshot 2024-10-15 at 12 15 10 PM" src="https://github.com/user-attachments/assets/d28d4f10-2db7-4226-9492-1182edec984a">

~~~//AREA OF RECTANGLE
#include<iostream>
using namespace std;
class MyClass{
    private:
    int l;
    int b;



    public:
int s,w;
void getinput()
         { 
            cout<<"Enter length and breadth"<<endl;
            cin>>s>>w;
         }

         void display()
         { int a;
         l=s;
         b=w;
    
            a = l*b;
         cout<<"Area of rectangle is: "<< a<< endl;
         }
};
int main(){
    
    MyClass obj1;
    obj1.getinput();
    obj1.display();

    return 0;
    }
~~~
  //output:
  ![image](https://github.com/user-attachments/assets/a546ef4f-554a-42ec-978d-8228f8bd4067)


~~~//DECONSTURCTOR
#include<iostream>
using namespace std;
class MyClass{
    public:
    ~MyClass(){
        cout<<"Destructor called! "<< endl;
    }
    MyClass(){
        cout<<"Constructor called!"<<endl;

    }
    };
    int main(){
        MyClass obj;
        return 0;
    }
~~~
//output:
<img width="226" alt="Screenshot 2024-10-15 at 12 15 51 PM" src="https://github.com/user-attachments/assets/f7615099-5c72-4627-9144-85441744f766">

# Conclusion:
In this experiment we learnt to define constructor, prameterized constructor, copy constructor, default arguments and deconsturctor
