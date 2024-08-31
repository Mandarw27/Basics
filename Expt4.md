# AIM:
To study and implement use of bitwise operators

# Bitwise Operators
Bitwise Operators are the operators that are used to perform operations on the bit level on the integers. While performing this operation integers are considered as sequences of binary digits. In C++, we have various types of Bitwise Operators.

Bitwise AND (&) Bitwise OR (|) Bitwise XOR (^) Bitwise NOT (~) Left Shift (<<) Right Shift (>>)

Bitwise AND (&) Bitwise AND operation is performed between two integers, It will compare each bit on the same position and the result bit will be set(1) only and only if both corresponding bits are set(1). The symbol which is used to perform bitwise AND operation is &.

Bitwise OR (|) If Bitwise OR operation is performed between two integers , It will compare each bit on same position and the result bit will be set(1) if any of corresponding bits are set(1). The symbol which is used to perform bitwise OR operation is |.

Bitwise XOR (^) If Bitwise XOR operation is performed between two integers , It will compare each bit on same position and the result bit will be set(1) if any of corresponding bits differ i.e. one of them should be 1 and other should be zero. The symbol which is used to perform bitwise XOR operation is ^.

Bitwise NOT (~) The Bitwise NOT operation is performed on a single number. It change the current bit to it’s complement , i.e. if current bit is 0 then in result it will be 1 and if current bit is 1 then it will become 0. It is denoted by the symbol ~.

Left Shift (<<) This operator shifts the bits of Integer to left side by specific number (As mentioned) . This left shift operation is equivalent to multiplying the integer by 2 power number of positions shifted. The symbol which is used to represent Left Shift Operator is <<.

Right Shift (>>) This operator shifts the bits of Integer to right side by specific number (As mentioned) . This right shift operation is equivalent to dividing the integer by 2 power number of positions shifted. The symbol which is used to represent Left Shift Operator is >>.


```javascript
//Mandar Wankhede
//23070123083

#include<iostream>
using namespace std;
int main()
{
    int a,b;
    cout<<"Enter first number: ";
    cin>>a;
    cout<<"Enter second number: ";
    cin>>b;
    cout<<"a==b: "<<(a==b)<<endl;
    return 0;
}
```
<img width="222" alt="Screenshot 2024-08-31 at 17 12 44" src="https://github.com/user-attachments/assets/844d98a3-8d0b-4462-b215-6e8bebaf4c27">

```javascript
#include<iostream>
using namespace std;
int main()
{
    int a,b;
    cout<<"Enter first number: ";
    cin>>a;
    cout<<"Enter second number: ";
    cin>>b;
    cout<<boolalpha;
    cout<<"a==b: "<<(a==b)<<endl;
    return 0;
}
```
<img width="248" alt="Screenshot 2024-08-31 at 17 15 01" src="https://github.com/user-attachments/assets/65f1537a-0deb-41d7-b6b2-624c7dd1cd95">

```javascript
#include<iostream>
using namespace std;
int main()
{
    bool a = true;
    bool b = false;
    cout<<boolalpha;
    cout<<"a&&b: "<<(a&&b)<<endl;
    return 0;
}
```
<img width="95" alt="Screenshot 2024-08-31 at 17 16 29" src="https://github.com/user-attachments/assets/ceae7e82-57cf-4738-b6a9-c99f355f13a0">

```javascript
#include<iostream>
using namespace std;
int main()
{
    int a,b;
    cout<<"Enter first number: ";
    cin>>a;
    cout<<"Enter second number: ";
    cin>>b;
    cout<<"a|b: "<<(a|b)<<endl;
    cout<<"a&b: "<<(a&b)<<endl;
    cout<<"a<<b: "<<(a<<b)<<endl;
    cout<<"ab: "<<(a>>b)<<endl;
    cout<<"~b: "<<(~b)<<endl;
    cout<<"a^b: "<<(a^b)<<endl;
    return 0;
}
```
<img width="333" alt="Screenshot 2024-08-31 at 17 18 04" src="https://github.com/user-attachments/assets/456d7328-117f-4b00-b64f-32359dfafd38">

```javascript
#include<iostream>
#include<bitset>
using namespace std;
int main()
{
    int a,b;
    cout<<"Enter first number: ";
    cin>>a;
    cout<<"Enter second number: ";
    cin>>b;
    cout<<"a|b: "<<bitset<4>(a|b)<<endl;
    cout<<"a&b: "<<bitset<4>(a&b)<<endl;
    cout<<"a<<b: "<<bitset<4>(a<<b)<<endl;
    cout<<"ab: "<<bitset<4>(a>>b)<<endl;
    cout<<"~b: "<<bitset<4>(~b)<<endl;
    cout<<"a^b: "<<bitset<4>(a^b)<<endl;
    return 0;
}
```
<img width="233" alt="Screenshot 2024-08-31 at 17 19 24" src="https://github.com/user-attachments/assets/5ddc31b2-3379-43c2-84ff-60221a84cfdf">

```javascript
#include<iostream>
 using namespace std;
 int main()
 {
     int a;
     cout <<"enter a number";
     cin>>a;
     if(a>=0)
         { cout <<"a is greater than 0";}
     else
     {cout<<"a is smaller than 0";}
     return 0;
}

```
<img width="211" alt="Screenshot 2024-08-31 at 17 20 40" src="https://github.com/user-attachments/assets/5368a96b-f199-4156-9db4-518bbfe7626d">

```javascript
#include <iostream>
#include <bitset>
using namespace std;

int main() {
    int num, set, reset;
    
    cout << "Enter a number: ";
    cin >> num;
    cout << "Enter the bit position to set (0 to 7): ";
    cin >> set;
    cout << "Enter the bit position to reset (0 to 7): ";
    cin >> reset;
    cout<<num<<" in binary is "<<bitset<8>(num)<<endl;
   
    int num_set = num | (1 << set);
    cout << "Result after setting bit number " <<set<< " is " << bitset<8>(num_set) << endl;
    
    int num_reset = num_set & ~(1 << reset);
    cout << "Result after resetting bit number " <<reset<< " is " << bitset<8>(num_reset) << endl;
    return 0;
}
```
<img width="403" alt="Screenshot 2024-08-31 at 17 22 07" src="https://github.com/user-attachments/assets/5e8a93d9-a4b8-49f1-8220-3abb98bb4635">
