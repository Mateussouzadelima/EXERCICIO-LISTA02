# EXERCICIO-LISTA02

1-

#include <stdio.h>
 
int main()
{
int fat, n;
printf("Insira um valor para o qual deseja calcular seu fatorial: ");
scanf("%d", &n);
 
for(fat = 1; n > 1; n = n - 1)
fat = fat * n;
 
printf("\nFatorial calculado: %d", fat);
return 0;
}

2-

#include <stdio.h>
#include <stdlib.h>

int main() {
  
  int i, x; 
  int div = 0;
  
  do {
    
    printf("Digite um número inteiro e positivo: ");
    scanf("%d", &x);
  } while (x <= 0);
  
  for (i = 1; i <= x; i++) {
    if (x % i == 0) { 
     div++;
    }
  }
    
  if (div == 2)
    printf("O número %d é primo!", x);
  else
    printf("O número %d não é primo!", x);

  return 0;
}


03-

#include <iostream>

using namespace std;

int main ()

{

int num, ant = 1, at = 1, pr;

cout << "Digite o numero de termos Fibonacci: ";

cin >> num;

for (int i = 1; i <= num; i++)

{

if (i == 1) cout << "0 ";

else if (i == 2 || i == 3) cout << "1 ";

else

{

pr = ant + at;

ant = at;

at = pr;

cout << " " << pr;

}

}

return 0;

}
