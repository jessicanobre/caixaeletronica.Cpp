Claro, aqui está uma documentação detalhada para o seu código C++:

# Documentação do Programa de Saque em Caixa Eletrônico

## Descrição Geral
Este programa em C++ é projetado para calcular a quantidade de notas de dinheiro necessárias para compor um valor específico de saque em um caixa eletrônico. O programa considera notas de 50, 20, 10 e 5.

## Bibliotecas Utilizadas
O programa utiliza duas bibliotecas padrão do C++:
- `iostream`: para entrada e saída de dados.
- `array`: para usar a estrutura de dados array.

## Funções

### Função `contaNotas`
Esta função recebe um valor de saque e retorna um array com a quantidade de cada nota necessária para compor esse valor. As notas consideradas são de 50, 20, 10 e 5.

#### Parâmetros
- `saque`: um inteiro que representa o valor total a ser sacado.

#### Retorno
- Retorna um array de inteiros onde cada elemento representa a quantidade de uma nota específica.

### Função `main`
Esta é a função principal do programa. Ela solicita ao usuário o valor a ser sacado, chama a função `contaNotas` para calcular a quantidade de cada nota e, em seguida, imprime esses valores.

## Como Usar
Para usar este programa, compile e execute o código. Quando solicitado, insira o valor que deseja sacar. O programa então imprimirá a quantidade de cada nota necessária para compor esse valor.
