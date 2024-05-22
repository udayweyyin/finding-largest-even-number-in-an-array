#include<stdio.h>
int main()
{
int x[10],y,largesteven;
y=0;
while(y<=9)
{
printf("Enter a number : ");
scanf("%d",&x[y]);
y++;
}
y=0;
while(y<=9)
{
if(x[y]%2==0)
{
break;
}
y++;
}
if(y==10)
{
printf("ALL ARE ODD\n");
}
else
{
largesteven=x[y];
y++;
while(y<=9)
{
if(x[y]%2==0&&x[y]>largesteven)
{
largesteven=x[y];
}
y++;
}
printf("LARGEST EVEN IS %d",largesteven);
}
return 0;
}
