#include<stdio.h>
int main()
{
    int n,i,j,temp;

    printf("Enter array size: ");
    scanf("%d",&n);

    int a[n];

    printf("Enter your data: ");

    for(i=0; i<n; i++)
        scanf("%d",&a[i]);

    //sorting

    for(i=0; i<n-1; i++)
    {
        for(j=0; j<n-i-1; j++)
        {
            if(a[j]<a[j+1])
            {
                temp=a[j];
                a[j]=a[j+1];
                a[j+1]=temp;
            }

        }
    }

    for(i=0; i<n; i++)

    printf("%d ",a[i]);



    printf("\n");
}
