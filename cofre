#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() {
    int tentativa, numeroSecreto, tentativasRestantes = 5;

    srand(time(NULL)); // inicializa o gerador aleatório
    numeroSecreto = rand() % 10 + 1; // número aleatório entre 1 e 10

    printf("=== CAÇA AO COFRE MISTERIOSO ===\n");
    printf("Um cofre está diante de você com um código secreto entre 1 e 10.\n");
    printf("Você tem 5 tentativas para descobrir o número e abrir o cofre.\n\n");

    while (tentativasRestantes > 0) {
        printf("Digite sua tentativa: ");
        scanf("%d", &tentativa);

        if (tentativa == numeroSecreto) {
            printf("🎉 Parabéns! Você acertou o código e abriu o cofre!\n");
            break;
        } else if (tentativa < numeroSecreto) {
            printf("O código é MAIOR que %d.\n", tentativa);
        } else {
            printf("O código é MENOR que %d.\n", tentativa);
        }

        tentativasRestantes--;
        printf("Tentativas restantes: %d\n\n", tentativasRestantes);
    }

    if (tentativasRestantes == 0 && tentativa != numeroSecreto) {
        printf("💥 Você esgotou suas tentativas! O código era: %d\n", numeroSecreto);
        printf("O cofre permanece fechado...\n");
    }

    return 0;
}
