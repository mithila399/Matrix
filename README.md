# Matrix 
#include <stdio.h>

int main()
{
    int a, b, c, d, e, f;

    printf("Enter the rows for matrix A: ");
    scanf("%d", &a);
    printf("Enter the columns for matrix A: ");
    scanf("%d", &b);

    printf("Enter the rows for matrix B: ");
    scanf("%d", &c);
    printf("Enter the columns for matrix B: ");
    scanf("%d", &d);

    int mA[a][b];
    int mB[c][d];

    printf("\n");
    printf("Your Matrices are: ");
    printf("A = %d x %d | B = %d x %d", a, b, c, d);

    printf("\n");

    for (int i = 0; i < a; i++)
    {
        for (int j = 0; j < b; j++)
        {
            printf("Enter Value for Matrix A[%d][%d]: ", i+1, j+1);
            scanf("%d", &mA[i][j]);
        }
    }

    for (int i = 0; i < c; i++)
    {
        for (int j = 0; j < d; j++)
        {
            printf("Enter Value for Matrix B[%d][%d]: ", i+1, j+1);
            scanf("%d", &mB[i][j]);
        }
    }

    printf("Matrix A is:");
    printf("\n");
    for (int i = 0; i < a; i++)
    {
        for (int j = 0; j < b; j++)
        {
            printf("%d\t", mA[i][j]);
        }
        printf("\n");
    }

    printf("\n");

    printf("Matrix B is:");
    printf("\n");
    for (int i = 0; i < c; i++)
    {
        for (int j = 0; j < d; j++)
        {
            printf("%d\t", mB[i][j]);
        }
        printf("\n");
    }

    printf("\n");
    printf("Matrix Addition of A and B is: ");
    printf("\n");

    for (int i = 0; i < a; i++)
    {
        for (int j = 0; j < b; j++)
        {
            int result[i][j];
            result[i][j] = mA[i][j] + mB[i][j];
            printf("%d\t", result[i][j]);
        }
        printf("\n");
    }

    printf("\n");
    printf("Matrix Subtraction of A and B is: ");
    printf("\n");

    for (int i = 0; i < a; i++)
    {
        for (int j = 0; j < b; j++)
        {
            int result[i][j];
            result[i][j] = mA[i][j] - mB[i][j];
            printf("%d\t", result[i][j]);
        }
        printf("\n");
    }


    return 0;
}
