\\Boa tarde ;)
#include <stdio.h>

void main() {
  char nomes[5][30];
  float notas[5];
  float media = 0;
  int i, indice;

  for (i = 0; i < 5; i++) {
    printf("\n Digite o NOME do aluno: ");
    scanf("%s", &nomes[i]);
    printf(" Digite a NOTA do aluno: ");
    scanf("%f", &notas[i]);

    media += notas[i];

    if ((i == 0) || (notas[i] > notas[indice])) {
      indice = i;
    }
  }
  printf("\n");
  media /= 5;
  printf("O aluno(a) %s tirou a nota mais alta (%.2f).\n\n", nomes[indice], notas[indice]);
  printf("Media de todas as notas: %.2f\n\n", media);
 
  system("\n PAUSE");
}

