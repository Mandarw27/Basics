
# EXPERIMENT 6:
## Aim: 
To study and implement C++ decision making statements (Loops)
## Theory: 
In C++, loops are used to execute a block of code repeatedly.

1. *for* loop: Ideal for iterating a known number of times. It includes initialization, condition, and increment/decrement in a single line.
2. Nested loop: A nested loop is simply a loop inside another loop.
3. Nested *for* loop: A for loop inside another for loop, often used for multidimensional data like matrices. Each inner loop completes all its iterations for every single iteration of the outer loop.
4. *while* loop: Executes a block of code repeatedly as long as the specified condition is true. The condition is checked before each iteration.
5. *do-while* loop: Similar to while, but the condition is checked after each iteration, ensuring the loop runs at least once.

These loops provide flexibility in controlling the flow of a program based on the needs of the task at hand.

~~~
CODE:

//Program 1 (For loop)
#include<iostream>
using namespace std;
int main() {
    int i;
    for(i=0;i<10;i++){
        cout<<"Hello world("<<i+1<<")"<<endl;
    }
}

//Program 2 (For loop to print sum)
#include<iostream>
using namespace std;
int main(){
    int sum=0, i, num;
    cout<<"enter the numbers for sum: ";
    
    cin>> num;
    for(i=1;i<=num;i++)
    {
         
        sum=sum+i;
          
    }
    cout<<"sum of first "<<num<<"natural numbers is "<<sum;
}

//Program 3 (For  loop)
#include<iostream>
using namespace std;
int main(){
    int num, i;
    cout<<"enter the end value";
    cin>>num;
    for(i=1;i<=num;i++)
    {
        cout<<i;
        
    }
}

//Program 4 (Nested-For loop)
 #include<iostream>
using namespace std;
int main(){
    int i, j;
    for(i=0;i<=3;i++)
    {
        for(j=0;j<=4;j++)
        {
            cout<<"*";
        }
        cout<<endl;
    }
}
    
//Program 5 (Printing inverted stars pattern)
#include<iostream>
using namespace std;
int main(){
    int i, j,rows=4;
    for(i=0;i<=rows;i++)
    {
        for(j=0;j<=i;j++)
        {
            cout<<" * ";
        }
        cout<<endl;
    }
}

//Program 6 (Printing star pattern)
#include<iostream>
using namespace std;
int main() 
{
    int i, j, k, rows=8;
    for(i=0;i<rows;i++)
    {
        for(j=rows-1;j>i;j--)
        {
            cout<<" ";
        }
        for(k=0;k<2*i+1;k++)
        {
            cout<<"*";
        }  cout<<endl;
    }
    
}
           
//Program 7 (Printing numbers n numbers)
#include<iostream>
using namespace std;
int main ()
{ int a,i=1;
    cout << "Enter end value: ";
    cin >> a;
    while( i <= a)
    { 
        cout<< " "<<i;
        i++;
    }
    return 0;
}

//Program 8 (Star pattern with numbers)
#include<iostream>
using namespace std;
int main()
{
    int i,j,row,n=1;
    std::cout<<"Enter the number of rows : ";
    std::cin>>row;
    for(i=0;i<row;i++)
    {
        for(j=0;j<i+1;j++)
        {
            cout<<n<<" ";
            n=n+1;
        }
        cout<<endl;
    }
    return 0;
}

//Program 9 (Floyd Series)
#include<iostream>
using namespace std;
int main()
{
    int row, a=1;
    cout<<"Enter the number of the rows: ";
    cin>>row;
    for(int i=0;i<row;i++)
    {
        for(int j=0;j<=i;j++)
        {
            cout<<a;
            a++;
        }
        cout<<endl;
    }
    return 0;
}

~~~

# Conclusion
In this experiment we learnt about loops and the various types of loops like for loop, while loop, loop and nested loops in C++.

## Experiment 6:

### Program 1 (For Loop):
![image](https://github.com/user-attachments/assets/f5efd38d-ccad-4c25-8dfd-42e8900c4f22)

### Program 2 (Sum of numbers using for loop):
![image](https://github.com/user-attachments/assets/5f37c749-5698-4750-ace3-c4a66460e7fc)

### Program 3 (For Loop):
![image](https://github.com/user-attachments/assets/54be064d-cfb1-44f8-b8b5-019cc29ef160)

### Program 4 (Nested-For loop):
![image](https://github.com/user-attachments/assets/30e64790-6655-4c34-a45d-6ba51cac5862)

### Program 5 (Printing inverted stars pattern):
![image](https://github.com/user-attachments/assets/36c57acc-f1ae-4ba3-8464-6e39dbdf76bd)

### Program 6 (Printing star pattern):
![image](https://github.com/user-attachments/assets/2d6093a3-9e86-4721-b23e-d1c70472aade)

### Program 7 (Printing n numbers):
![image](https://github.com/user-attachments/assets/518abdca-44ef-4a7b-86d6-e63e544be3ee)

### Program 8 (Star pattern with numbers):
![image](https://github.com/user-attachments/assets/f2c4d5e6-4df9-46c5-96ad-2318ac40ca23)

### [Program 9 (Floyd Series):
![image](https://github.com/user-attachments/assets/8b7051f5-097c-4281-8642-4a49ce2723e6)
