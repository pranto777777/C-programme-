#include <stdio.h>
#include<math.h>
int fac (int);
int main() {
    int a,b,i=0,x;
    float c=1;
    scanf("%d",&a);
    scanf("%d",&x);
   for(i=2;i<=a;i=i+2) 
 c=c-pow(-x,i)/fac(i);;   
printf("%f",c);
    
    return 0;
}
int fac(int a)
{if (a==0)
return (1);
    int c=a*fac(a-1);
    return (c);
}
