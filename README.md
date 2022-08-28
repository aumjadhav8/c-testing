#include <stdio.h>
#include <math.h>

void main()
{
    int n, i;
    float a[20],*ptr,mean,sum = 0,sumstd = 0,std;

    printf ("Enter the number of elements (n) : \n");
    scanf ("%d",&n);

    printf ( "Enter the value of elements : \n");
    for (i=0;i<n;i++)
    {
        scanf("%f", &a[i]);
    }

    // finding the sum

    for (i=0;i<n;i++)
    {
        sum = sum + ptr[i];
    }

    mean = sum/n;

    // finding sumstd

    for (i=0;i<n;i++)
    {
        sumstd = sumstd + pow((ptr[i]-mean),2);
    }

    // standard deviation 

    std = sqrt(sumstd/n);

    printf ("The sum of the elements is : ", sum);
    printf ("The mean of the elements is : ", mean);
    printf ("The standard deviation of the elements is : ", std);

}
