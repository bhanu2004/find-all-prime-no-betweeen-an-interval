/ find-all-prime-no-betweeen-an-interval
#include <iostream>
#include <math.h>

using namespace std;
int prime(int n){
      for(int i=2;i<=sqrt(n);i++){
       if(n%i==0){
      
           return 1;
           
       }
       
   }
   return 0;
}

int main()
{   
    int first,last;
   cout<<"enter the two numbers: ";
   cin>>first>>last;
   for(int i=first;i<=last;i++){
       if(prime(i)==0)
            cout<<i<<" ";
   }
