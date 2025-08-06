# GetElements-in-array

#include<bits/stdc++.h>   
using namespace std;
void getElements(int arr[],int n)
{
    if(n==0 || n==1)
       cout<<-1<<" "<<-1<<endl;  
    sort(arr,arr+n);
    int small=arr[1];
    int large=arr[n-2];
    cout<<"Second smallest is "<<small<<endl;
    cout<<"Second largest is "<<large<<endl;
}
int main()
{
    int arr[]={1,6,8,3,7,2,9,4};
    int n=sizeof(arr)/sizeof(arr[0]);
    getElements(arr,n);
    return 0;
}
