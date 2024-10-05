# switch.java
Este programa em Java demonstra o uso da estrutura de controle switch, que é utilizada para tomar decisões com base no valor de uma variável.

Descrição do Código

Este programa em Java demonstra o uso da estrutura de controle switch, que é utilizada para tomar decisões com base no valor de uma variável.
Estrutura do Código:

    switch: O switch é uma alternativa ao uso de múltiplos blocos if-else, permitindo comparar o valor de uma variável com diferentes casos (case). Dependendo do valor da variável, o programa executa o código correspondente ao case que combina com o valor da variável.

    case: Cada case representa uma possível escolha baseada no valor da variável avaliada. Quando o valor da variável opcoes coincide com um dos cases, o código correspondente será executado.

    break: A instrução break é usada para sair da estrutura switch após a execução de um case. Sem o break, o programa continua executando os próximos cases, mesmo que eles não correspondam ao valor original, o que pode gerar comportamentos inesperados. Isso é chamado de "fall-through".

Opções no Código:

Neste exemplo, a variável opcoes é definida como 5, e o programa avalia este valor com base nos cases definidos:

    Case 1: Exibe "Abrir uma nova conta".
    Case 2: Exibe "Abrir uma conta existente".
    Case 3: Exibe "Crédito Imobiliário".
    Case 4: Exibe "Nenhuma opção foi selecionada".
    Default: Se o valor não corresponder a nenhum dos cases, o bloco default seria executado. No entanto, neste código, o default está vazio.

Comportamento ao Remover um break:

Se o break for removido de um case, o programa continuará executando os próximos cases, independentemente do valor da variável. Por exemplo, se o break após o Case 1 for removido, e o valor de opcoes for 1, o programa exibirá:

    "Abrir uma nova conta"
    "Abrir uma conta existente" (mesmo que opcoes seja 1)

Esse comportamento é chamado de "fall-through", e pode ser útil em alguns cenários, mas geralmente não é desejado quando cada case deve ser independente.
