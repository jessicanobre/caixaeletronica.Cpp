
# Documentação do Programa de Saque em Caixa Eletrônico

## Descrição Geral
Este programa em C++ é projetado para calcular a quantidade de notas de dinheiro necessárias para compor um valor específico de saque em um caixa eletrônico. O programa considera notas de 50, 20, 10, 5 e 2.

## Bibliotecas Utilizadas
O programa utiliza duas bibliotecas padrão do C++:
- `iostream`: para entrada e saída de dados.
- `array`: para usar a estrutura de dados array.

## Funções

### Função `contaNotas`
Esta função recebe um valor de saque e retorna um array com a quantidade de cada nota necessária para compor esse valor. As notas consideradas são de 50, 20, 10, 5 e 2.

#### Parâmetros
- `saque`: um inteiro que representa o valor total a ser sacado.

#### Retorno
- Retorna um array de inteiros onde cada elemento representa a quantidade de uma nota específica.

### Função `main`
Esta é a função principal do programa. Ela solicita ao usuário o valor a ser sacado, chama a função `contaNotas` para calcular a quantidade de cada nota e, em seguida, imprime esses valores.

## Como Usar
Para usar este programa, compile e execute o código. Quando solicitado, insira o valor que deseja sacar. O programa então imprimirá a quantidade de cada nota necessária para compor esse valor.

## Erros que o código possui 

1. **Tratamento de Entrada Inválida**: O código atualmente não verifica se a entrada do usuário é válida. Por exemplo, se o usuário inserir um valor não numérico ou um número negativo, o programa pode não funcionar corretamente. Uma verificação de entrada poderia ser adicionada para garantir que o valor de saque seja um número inteiro positivo.

2. **Notas Indisponíveis**: O código não considera a situação em que certas notas podem não estar disponíveis. Por exemplo, se o caixa eletrônico não tiver notas de 2, o programa ainda tentará calcular a quantidade de notas de 2. Uma possível melhoria seria adicionar uma verificação para garantir que apenas as notas disponíveis sejam consideradas.

3. **Valores de Notas Codificados**: Os valores das notas estão codificados diretamente na função `contaNotas`. Isso torna o código menos flexível se quisermos mudar os valores das notas ou adicionar novas notas. Uma possível melhoria seria armazenar os valores das notas em um array ou outra estrutura de dados, para que possam ser facilmente modificados ou expandidos.

4. **Tratamento de Valores Não Divisíveis**: O código não trata valores de saque que não são divisíveis pelas notas disponíveis. Por exemplo, se o usuário tentar sacar 3, o programa não será capaz de fornecer um resultado válido, pois não há notas de 1. Uma possível melhoria seria adicionar uma mensagem de erro ou aviso para esses casos.
