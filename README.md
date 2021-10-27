# new
#include <iostream>
#include<conio.h>
using namespace std; 
int main()
{
    int arr[10];
    int  i, j, temp;
    cout<<"Enter elements in array: ";
    for(i=0; i<10; i++)
    {
        cin>>arr[i];
    }
    for(i=0; i<10; i++)
    {
        for(j=i+1; j<10; j++)
        {
            if(arr[j] < arr[i])
            {
                temp = arr[i];
                arr[i] = arr[j];
                arr[j] = temp;
            }
        }
    }
    cout<<"Elements of array in sorted form:"<<endl;
    for(i=0; i<10; i++)
    {
        cout<<arr[i]<<endl;
    }
 getch();
    return 0;
}
