#include<iostream>
#include<cmath>
using namespace std;

int main()
{
    int n,key;
    cin>>n;

    int arr[n];

    for(int i=0;i<n;i++)
    cin>>arr[i];

    cin>>key;

    int step=sqrt(n);
    int prev=0;

    while(arr[min(step,n)-1]<key)
    {
        prev=step;
        step+=sqrt(n);

        if(prev>=n)
        {
            cout<<"Not Found";
            return 0;
        }
    }

    while(arr[prev]<key)
    {
        prev++;

        if(prev==min(step,n))
        {
            cout<<"Not Found";
            return 0;
        }
    }

    if(arr[prev]==key)
    cout<<"Found at "<<prev;
    else
    cout<<"Not Found";

    return 0;
}
