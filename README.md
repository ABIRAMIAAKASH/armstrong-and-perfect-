# armstrong-and-perfect-
my first project
#include <stdio.h>
int count (int a)
{
    int c=0;
    while(a)
    {
        c++;
        a/=10;
    }
return c;
}
int power(int n, int m)
 {     int p=1;
       while(m--)
      {
       p*=n;
      }
     return p;
 }

    


int main()
{
   int n,d,s=0,t,m,i,b=0;
scanf("%d",&n);
m=n;
t=n;
d=count(n);

while(n)
{
    s+=power(n%10,d);
    n/=10;
}
if(t==s)
  printf("armstrong\n");
 else
 printf("not armstrong");
 for(i=1;i<=m/2;i++)
        {
            if(m%i==0)
            b+=i;
        }
printf(m==b?"perfect\n":"not perfect\n");    

    return 0;
}

