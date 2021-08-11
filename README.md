# Codes
This consists of the various codes right from basic I've learnt throughout my life in various languages.

MULTIPLICATION OF MATRICES

#include<stdio.h>
#include<stdlib.h>
main()
{
int r1;
int c1;
int r2;
int c2;
int i;
int j;
int k;
int A[20][20];
int B[20][20];
int C[20][20];
printf("Enter the no of rows of Matrix A\n");
scanf("%d",&r1);
printf("Enter the no of columns of Matrix A\n");
scanf("%d",&c1);
printf("Enter the no of rows of Matrix B\n");
scanf("%d",&r2);
printf("Enter the no of rows of Matrix B\n");
scanf("%d",&c2);
if(!(r2==c1))
{
printf("Invalid matrix");
exit(1);
}
printf("Enter the elements of matrix A\n");
for(i=0;i<r1;i++)
{
for(j=0;j<c1;j++)
{printf("Enter the element\n");
scanf("%d",&A[i][j]);
}
}
printf("Enter the elements of matrix B\n");
for(i=0;i<r2;i++)
{
for(j=0;j<c2;j++)
{printf("Enter the element\n");
scanf("%d",&B[i][j]);
}
}
printf("Matrix A\n");
for(i=0;i<r1;i++)
{
for(j=0;j<c1;j++)
{
printf("%d ",A[i][j]);
}
printf("\n");
}
printf("\n");

printf("Matrix B\n");
for(i=0;i<r1;i++)
{
for(j=0;j<c1;j++)
{
printf("%d ",B[i][j]);
}
printf("\n");
}

printf("\n");
for(i=0;i<r1;i++)
{
for(j=0;j<c2;j++)
{C[i][j]=0;
for(k=0;k<c1;k++)
{C[i][j]+=A[i][k]*B[k][j];
}
}
}
printf("\n");
for(i=0;i<r1;i++)
{
for(j=0;j<c1;j++)
{
printf("%d ",C[i][j]);
}
printf("\n");
}
}
