#include <stdio.h>
#define MAX 100

int main() {
  int n, i, v[MAX]; //Declaração das variáveis n é o tamanho, i é usado pelo comando for e v é o vetor

  printf("Digite o comprimento da sequencia: ");
  scanf("%d", &n); //leitura da variável

  printf("Digite uma sequencia com %d nC:meros inteiros: ", n);
  for (i = 0; i < n; i++) //i vai começar no 0 e vai até alcançar o valor máximo de n, parando antes de chegar nele. No fim sempre somando mais um
    scanf("%d", &v[i]);
  for (i = n-1; i >= 0; i--) //i vai começar no valor total de n-1 e vai até alcançar 0, mas agora lendo o vetor final
    printf("%d ", v[i]);
  printf("\n"); //quebra de linha
  return 0;
}
