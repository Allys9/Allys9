#include <stdio.h>

int main() {
  int numero, suma = 0, i;
  printf("Introduce un numero: ");
  scanf("%d", &numero);
  for (i = 1; i <= numero / 2; i++) {
    if (numero % i == 0) {
      suma += i;
    }
  }
  if (suma == numero) {
    printf("%d es un numero perfecto.\n", numero);
  } else {
    printf("%d no es un numero perfecto.\n", numero);
  }
  return 0;
}
