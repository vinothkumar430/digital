# digital
#include<stdio.h>
main()
{
int i,j,n,a[100];
printf("Enter how many elements you want\n");
scanf("%d",&n);
printf("Enter the elements\n");
for(i=0;i<n;i++)
scanf("%d",&a[i]);
//bubble sort
for(i=0;i<n;i++)
{
for(j=i-1;j<n;j++)
{
if(a[i]>a[j])
{
temp=a[j];
a[j]=a[i];
a[i]=temp;
}
}
}
//printing the elements in ascending order
for(i=0;i<n;i++)
printf("%d",a[i]);
}

