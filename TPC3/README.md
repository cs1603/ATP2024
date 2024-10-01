O objetivo do código é implementar um jogo interativo, onde um jogador compete contra o computador para retirar fósforos, utilizando uma estratégia que 
aumente a probabilidade de alcançar a vitória.Além disso, tanto o computador como o jogador têm como objetivo evitar ser o último a retirar o fósforo de um conjunto inicial de 21 fósforos. 
O jogo envolve dois participantes: o jogador e o computador. Cada um tem o seu momento para jogar e pode retirar entre 1 a 4 fósforos, sendo que o participante que retirar o último fósforo perde o jogo.
O jogo começa com a definição do número inicial de fósforos (n_fosforos = 21). Uma variável (jogador_per) é utilizada para determinar o vencedor, sendo inicializada como vazia.
O jogo continua enquanto houver fósforos disponíveis (n_fosforos > 0) e nenhum dos jogadores tenha perdido (jogador_per == ""). Dentro do loop, ocorrem as jogadas alternadas entre o jogador e o computador.
O jogador deve inserir um valor de 1 a 4, indicando quantos fósforos deseja retirar. O código verifica se a escolha é válida, ou seja, se o valor está entre 1 e 4 e se não é maior do que o número de fósforos restantes. O valor é então subtraído ao total de fósforos disponíveis e o número restante é exibido.
Se ainda restarem fósforos após a jogada do jogador, o computador faz a sua jogada. A lógica do computador consiste em escolher estrategicamente quantos fósforos deve retirar. Se a quantidade de fósforos restantes menos 1 for divisível por 5 ((n_fosforos - 1) % 5 == 0), o computador escolhe aleatoriamente entre 1 e 4 fósforos. Caso contrário, ele retira (n_fosforos - 1) % 5 fósforos, visando maximizar suas chances de vitória.
Se o jogador retira o último fósforo, o computador é declarado vencedor e vice-versa. O resultado é exibido ao final da execução do código.


A estratégia do computador é baseada na tentativa de deixar o jogador numa situação desfavorável. Ao calcular (n_fosforos - 1) % 5, ele garante que o número de fósforos restantes depois da sua jogada seja uma quantidade que favoreça a sua vitória, fazendo o jogador ficar com menos opções favoráveis.

O jogo implementado utiliza uma combinação de interação com o utilizador e lógica estratégica para o computador, o que torna a experiência mais desafiadora. O jogador precisa de escolher cuidadosamente quantos fósforos retirar para não acabar por perder. 

