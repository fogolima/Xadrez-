#include <stdio.h>

int main() {
    // Definindo o número de casas que cada peça pode se mover
    int casas_Torres = 5;   // Torre pode mover 5 casas para a direita
    int casas_Bisbo = 5;    // Bispo pode mover 5 casas na diagonal superior direita
    int casas_Rainha = 8;   // Rainha pode mover 8 casas para a esquerda

    // Movimento da Torre
    printf("Movimento da Torre:\n");
    for (int i = 0; i < casas_Torres; i++) {
        printf("Direita\n");  // Imprime "Direita" para cada casa que a Torre se move
    }

    // Movimento do Bispo
    printf("Movimento do Bispo:\n");
    int i = 0;
    while (i < casas_Bisbo) {
        printf("Cima Direita\n");  // Imprime "Cima Direita" para cada casa que o Bispo se move
        i++;  // Incrementa o contador
    }

    // Movimento da Rainha
    printf("Movimento da Rainha:\n");
    i = 0;  // Reinicializa o contador
    do {
        printf("Esquerda\n");  // Imprime "Esquerda" para cada casa que a Rainha se move
        i++;  // Incrementa o contador
    } while (i < casas_Rainha);  // Continua o loop enquanto o contador for menor que o número de casas

    return 0;  // Retorna 0 indicando que o programa terminou com sucesso
}
