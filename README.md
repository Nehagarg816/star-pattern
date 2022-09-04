# star-pattern
This is a program for printing of star pattern in straight and reverse counting using loops.

#include <stdio.h>
int main()
{
    int choice, i, j, n, a;
    printf("Press 1 for Triangular star pattern");
    printf("\nPress 2 for Reverse star pattern");
    printf("\nEnter your choice:");
    scanf("%d", &choice);
    switch (choice)
    {
    case 1:
        printf("Enter no. of lines pattern to be printed:");
        scanf("%d", &n);
        for (i = 0; i < n; i++)
        {
            for (j = 0; j <= i; j++)
            {
                printf("*");
            }
            printf("\n");
        }

        break;

    case 2:
        printf("Enter no. of lines pattern to be printed:");
        scanf("%d", &a);
        for (i = a; i > 0; i--)
        {
            for (j = i; j > 0; j--)
            {
                printf("*");
            }
            printf("\n");
        }
        break;

    default:
        printf("Invalid choice");
        break;
    }
    return 0;
}
