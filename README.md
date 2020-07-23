#include<stdio.h>
#include<cs50.h>

int main(void)
{
    int n;
    do
    {
    n = get_int("Height:");
    }
    while(n < 1 || n > 8);
    for( int i = 0; i < n; i++)
    {
        for(int a = n - 1; a > i; a--)
        {
            printf(" ");
        }
        for( int j = i; j >=0; j--)
        {
        printf("#");
        }
        printf("  ");
        for( int k = i; k >=0; k--)
        {
            printf("#");
        }
        printf("\n");
    } 
}
