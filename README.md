# miniCalculadora
Operações matemáticas simples 
#include <stdio.h>
#include <stdlib.h>
int main()
{
	int valorSwitch, s1, s2, soma, n1, n2, sub;
	float d1, d2, div, m1, m2, multi;
	int voltarInicio;
	do{
	printf("ESCOLHA A OPCAO QUE VOCE DESEJA\n 1-SOMA\n 2-SUBTRACAO\n 3-DIVISAO\n 4-MULTIPLICACAO\n 5-SAIR\n");
	scanf("%i", &valorSwitch);
	
	switch (valorSwitch)
	{
	case 1:
	
		system ("cls"); 
		printf("SOMA\n");
		printf("DIGITE DOIS VALORES!\n");
		setbuf(stdin, NULL);
		scanf ("%i", &s1);
		scanf ("%i", &s2);
		soma = s1 + s2;
		printf("A SOMA ENTRE %d e %d eh = %d\n", s1, s2, soma);
		
		break;
	case 2:
		system ("cls"); 
		printf("\nSUBTRACAO\n");
		printf("DIGITE DOIS VALORES!\n");
		setbuf(stdin, NULL);
		scanf ("%i", &n1);
		scanf ("%i", &n2);
		sub = n1 - n2;
		printf("A SUBTRACAO ENTRE %d e %d eh = %d\n", n1, n2, sub);
		break;
	case  3:
		system ("cls"); 
		printf("DIVISAO\n");
		printf("DIGITE O VALOR QUE VOCE QUER DIVIDIR!\n");
		setbuf(stdin, NULL);
		scanf("%f", &d1);
		printf("EM QUANTAS VEZES GOSTARIA DE DIVIDIR?\n");
		setbuf(stdin, NULL);
		scanf("%f", &d2);
		div = d1 / d2;
		printf(" A DIVISAO ENTRE %.2f E %.2f eh = %.2f\n", d1, d2, div);
		break;
	case 4:
		system ("cls"); 
		printf("\nMULTIPLICACAO\n");
		printf("DIGITE O VALOR QUE VOCE QUER MULTIPLICAR\n");
		setbuf(stdin, NULL);
		scanf ("%f", &m1);
		printf("EM QUANTAS VEZES GOSTARIA DE MULTIPLICAR ESSE VALOR?\n");
		setbuf(stdin, NULL);
		scanf ("%f", &m2);
		multi = m1 * m2;
		printf("A MULTIPLICACAO ENTRE %.2f E %.2f EH = %.2f\n", m1, m2, multi);
		break;
	case 5:
		system ("cls");
		return 0;
	default :
		system ("cls"); 
		printf("POR FAVOR TENTE DE NOVO!\n");
		break;
	}
	printf("\n VOCE GOSTARIA DE VOLTAR AO INICIO? \n");
		printf("1-SIM\n2-NAO\n");
		setbuf(stdin, NULL);
		scanf("%i", &voltarInicio);
		system ("cls"); 
	}
	while(voltarInicio == 1);
	system("pause");
	return 0;
}
