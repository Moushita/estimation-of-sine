# estimation-of-sine
A code to calculate the value of sine as derived from Taylor Series Expansion.
#include <iostream.h>
#include <constream.h>
void main()
{
int i,x,k,temp=1;
float sine=0,term;
cout<<"Enter the number of terms(k)";
cin>>k;
cout<<"Enter the angle(x)";
cin>>x;
for(i=0;i<k;i++)
{
temp*=i;
term=((pow(x,i)/temp);
sine+=term;
}
cout<<"The sine value for angle "<<x<<" for "<<k<<" iterations is "<<sine;
getch();
}
