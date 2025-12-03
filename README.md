# project-14
Matrix Addition Program
#include <stdio.h>

int main() {
    int a[10][10], b[10][10], sum[10][10];
    int r, c;

    printf("Enter rows and columns: ");
    scanf("%d %d", &r, &c);

    printf("Enter elements of matrix A:\n");
    for (int i = 0; i < r; i++)
        for (int j = 0; j < c; j++)
            scanf("%d", &a[i][j]);

    printf("Enter elements of matrix B:\n");
    for (int i = 0; i < r; i++)
        for (int j = 0; j < c; j++)
            scanf("%d", &b[i][j]);

    printf("\nSum of matrices:\n");
    for (int i = 0; i < r; i++) {
        for (int j = 0; j < c; j++) {
            sum[i][j] = a[i][j] + b[j][j];
            printf("%d ", sum[i][j]);
        }
        printf("\n");
    }

    return 0;
}
