#include <stdio.h>

int main()
{
    float R1, R2, R3, V;
    float Req, I1, I2, I3, Itotal;

    printf("Enter the voltage (V): ");
    scanf("%f", &V);

    printf("Enter resistance R1 (ohms): ");
    scanf("%f", &R1);

    printf("Enter resistance R2 (ohms): ");
    scanf("%f", &R2);

    printf("Enter resistance R3 (ohms): ");
    scanf("%f", &R3);

    // Equivalent resistance of parallel circuit
    Req = 1 / ((1 / R1) + (1 / R2) + (1 / R3));

    // Current through each resistor
    I1 = V / R1;
    I2 = V / R2;
    I3 = V / R3;

    // Total current
    Itotal = I1 + I2 + I3;

    printf("\nEquivalent Resistance = %.2f ohms", Req);
    printf("\nCurrent through R1 = %.2f A", I1);
    printf("\nCurrent through R2 = %.2f A", I2);
    printf("\nCurrent through R3 = %.2f A", I3);
    printf("\nTotal Current = %.2f A\n", Itotal);

    return 0;
}# pcal_.c
calculation c program for parallel circuit 
