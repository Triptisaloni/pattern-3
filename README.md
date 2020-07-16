# pattern-3 in c
     1
   2 3 2
  3 4 5 4 3
 4 5 6 7 6 5 4
5 6 7 8 9 8 7 6 5


#include<stdio.h>
#include<conio.h>
void main()
{
    int i,j,k,l,e,d,x;
    for(i=1;i<=5;i++)
    {
        x=i;
        for(j=5;j>=i;j--)
        {
            printf(" ");
        }
       for(k=1;k<=i;k++)
       {
           printf("%d",x);
           x=x+1;
       }
       d=i%2;
       e=i+d;
       for(l=2;l<=i;l++)
       {
          while(e>=i)
          {
              printf("%d",e);
              e--;
          }
       }
       printf("\n");
    }
    getch();
}
