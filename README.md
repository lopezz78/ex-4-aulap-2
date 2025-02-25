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

 //(DESAFIO) Construir um programa que faz a leitura de duas
//notas de um aluno, N1 e N2, e os respectivos pesos, P1 e P2. O
//programa deve calcular a média ponderada alcançada por aluno
//e apresentar:
//• A mensagem "Aprovado", se a média alcançada for maior ou
//igual a sete;
//• A mensagem "Reprovado", se a média for menor do que
//sete;
//• A mensagem "Aprovado com Distinção", se a média for igual
//a dez.

#include <stdlib.h>
#include <stdio.h>

int main()

 {
    float N1, N2, P1, P2, mf;

    printf("\n\tNota 1: ");
    scanf("%f", &N1);

    printf("\n\tNota 2: ");
    scanf("%f", &N2);

    printf("\n\tPeso 1: ");
    scanf("%f", &P1);

    printf("\n\tPeso 2: ");
    scanf("%f", &P2);

    mf = (N1*P1) + (N2*P2)/(P1+P2);


    if (mf >= 7)
    {
        printf("\n\tAprovado! ");
    }
    
    else
    {
        if (mf  7)
    }
 }
