Este código implementa uma aplicação para a manipulação de listas de inteiros, começando por apresentar um menu interativo para o utilizador. 
O programa permite criar listas aleatórias, ler listas inseridas manualmente, calcular soma, média, encontrar o maior e o menor elemento, 
verificar se a lista está ordenada, de forma decrescente ou crescente, e procurar elementos específicos fornecidos pelo utilizador. 
A função principal (main()) mantém a interação contínua até que o utilizador escolha a opção "0", que signifca sair.
Assim que o programa começa a rodar, o utilizador encontra de imediato um menu de opções que lhe permite realizar algumas operações. 
O menu é bastante claro e intuitivo para que o utilizador não se confunda.

Principais Funcionalidades:
Criação e Manipulação de Listas: Permite criar listas aleatórias ou lidas através da interação computador-utilizador.
Cálculos: Realiza operações como soma, média, encontrar maior e menor elemento.
Verificações de Ordem: Confere se a lista está ordenada em ordem crescente ou decrescente.
Procura de Elemento: Permite procurar o elemento que o utilizador pede.


Durante a elaboração do código, algumas dificuldades foram enfrentadas e superadas:

Controlo do Fluxo do Programa: Inicialmente, utilizava o comando break para finalizar o loop principal. A dificuldade foi superada reformulando a 
estrutura do while para uma condição de paragem clara (opcao != "0"), tornando o fluxo do programa mais intuitivo.

Verificação de Ordem: Inicialmente, a verificação da ordem crescente e decrescente não devolvia valores claros para reutilização posterior. 
O problema foi resolvido ao ajustar as funções para comparar diretamente a lista dada com a sua versão ordenada, fornecendo uma resposta de "Sim" ou "Não".





