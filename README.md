# ex-4-aulap-2

//Faça um programa que calcule o reajuste do salário de um
//funcionário. Considere que o funcionário deverá receber um
//reajuste de 15%, caso seu salário seja menor que R$500,00; se o
//salário for maior ou igual a R$500,00, mas menor ou igual a
//R$1000,00, seu reajuste será de 10%; caso seja ainda maior que
//R$1000,00, o reajuste deverá ser de 5%.

#include <stdlib.h> #include <stdio.h>

int main()

 {
    float salario;

        printf("\n\tDigite o valor do salario: ");
        scanf("%f", &salario);

    if (salario<500)
    {
        salario = salario*1.15;
        printf("\n\tReajustado: %.2f ", salario);
    }

    else
    {
        if (salario>=500 && salario<=1000)
        {
            salario = salario*1.1;
            printf("\n\tReajustado: %.2f ", salario);
        }
        else
        {
            if (salario>1000)
            {


            salario = salario*1.05;
            printf("\n\tReajustado: %.2f ", salario);
            }
        }
    }
 }
