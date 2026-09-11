# zparameters.p
z parameters calculation in c program 
#include <stdio.h>

int main()
{
    float V1_1, V2_1, I1, V1_2, V2_2, I2;
    float Z11, Z21, Z12, Z22;

    printf("Z-Parameter Calculation\n");

    printf("\nEnter V1, V2 and I1 for I2 = 0:\n");
    scanf("%f %f %f", &V1_1, &V2_1, &I1);

    printf("\nEnter V1, V2 and I2 for I1 = 0:\n");
    scanf("%f %f %f", &V1_2, &V2_2, &I2);

    Z11 = V1_1 / I1;
    Z21 = V2_1 / I1;

    Z12 = V1_2 / I2;
    Z22 = V2_2 / I2;

    printf("\nZ-Parameters:\n");
    printf("Z11 = %.2f Ohms\n", Z11);
    printf("Z12 = %.2f Ohms\n", Z12);
    printf("Z21 = %.2f Ohms\n", Z21);
    printf("Z22 = %.2f Ohms\n", Z22);

    return 0;
}