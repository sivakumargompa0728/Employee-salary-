#include <stdio.h>

int main() {
    int empId;
    char name[50];
    float basic, hra, da, pf, gross, net;

    // Input details
    printf("Enter Employee ID: ");
    scanf("%d", &empId);

    printf("Enter Employee Name: ");
    scanf("%s", name);

    printf("Enter Basic Salary: ");
    scanf("%f", &basic);

    // Calculations
    hra = 0.20 * basic;   // 20% HRA
    da = 0.10 * basic;    // 10% DA
    pf = 0.05 * basic;    // 5% PF deduction

    gross = basic + hra + da;
    net = gross - pf;

    // Output
    printf("\n----- Employee Salary Details -----\n");
    printf("Employee ID   : %d\n", empId);
    printf("Employee Name : %s\n", name);
    printf("Basic Salary  : %.2f\n", basic);
    printf("HRA (20%%)     : %.2f\n", hra);
    printf("DA (10%%)      : %.2f\n", da);
    printf("PF (5%%)       : %.2f\n", pf);
    printf("Gross Salary  : %.2f\n", gross);
    printf("Net Salary    : %.2f\n", net);

    return 0;
}
