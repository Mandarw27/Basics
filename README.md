# Exp8

```javascript
//Mandar Wankhede
//23070123083
//EntcB1
//program 1
#include <iostream>
using namespace std;
int main() 
{
    int r,c,i,j;
    cout<<"enter number of rows";
    cin>>r;
    cout<<"Enter number of coloumns";
    cin>>c;
    int a[r][c];
    for(i=0;i<r;i++)
    {
        for(j=0;j<c;j++)
        {
            cout<<"Enter element ("<<i<<","<<j<<")";
            cin>>a[i][j];
        }
            
    }
    for(i=0;i<r;i++)
    {
        for(j=0;j<r;j++)
        {
            cout<<"  "<<a[i][j];
        }
        cout<<endl;
    }
    return 0;
}
//Mandar Wankhede
//Program2

#include <iostream>
using namespace std;
int main() {
   int r,c,i,j,x,z;
    cout<<"enter number of rows of m1";
    cin>>r;
    cout<<"Enter number of coloumns of m1";
    cin>>c;
    cout<<"enter number of rows of m2";
    cin>>x;
    cout<<"enter number of rows of m2";
    cin>>z;
    int a[r][c];
    for(i=0;i<r;i++)
    {
        for(j=0;j<c;j++)
        {
            cout<<"Enter element a("<<i<<","<<j<<")";
            cin>>a[i][j];
        }
    }
        
    int b[x][z];
    for(i=0;i<r;i++)
    {
        for(j=0;j<c;j++)
        {
            cout<<"Enter element b("<<i<<","<<j<<")";
            cin>>b[i][j];
        }
    }
    int d[r][c];
    for(i=0;i<r;i++)
    {
        for(j=0;j<c;j++)
        {
             d[i][j]=a[i][j]+b[i][j];
        }
    }
    cout<<"The addition of the 2 matrices is"<<endl;
      for(i=0;i<r;i++)
    {
        for(j=0;j<c;j++)
        {
            cout<<" "<<d[i][j];
        }
        cout<<endl;
    }
        

  
}

```
![image](https://github.com/user-attachments/assets/e9119e4a-76b0-4e9a-a59d-023093a6c7ca)

