#include<stdio.h>
#include<conio.h>

void main(){
    int i,j,n, temp;
    int a[10] = {5,2,10,11,6,9,8,7,3,1};
    n = 10;
    for(i=0;i<n-1;i++)
    {
        for(j=0;j<n-i-1;j++)
        {
            if(a[j]>a[j+1])
            {
                temp = a[j];
                a[j] = a[j+1];
                a[j+1] = temp;
            }
        }
    }
    printf("BUBBLE SORT IS IN PROGRESS........\n");
    printf("The sorted orer is\n");
    for(i=0;i<n;i++)
    {
        printf("%d| ", a[i]);
    }
}
