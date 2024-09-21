Neste trabalho foram implementados dois jogos, um onde o jogador tenta adivinhar um número gerado pelo computador, e outro onde o computador tenta adivinhar um número que o jogador tem em mente. Façamos uma análise detalhada do raciocínio que utilizei para pôr o jogo a funcionar:

1. Jogo onde o jogador adivinha o número do computador

O computador gera um número aleatório entre 0 e 100 usando random.randrange(0,100).
O jogador tenta adivinhar o número, e a cada tentativa o jogo dá uma dica se o número é maior ou menor do que o palpite, pois assim que for igual o jogo termina.
O loop continua até o jogador acertar o número, e o total de palpites é contabilizado por um contador.
Raciocínio:


2. Jogo onde o computador adivinha o número do jogador

O computador tenta adivinhar um número que o jogador tem em mente. O jogador dá dicas ('m' para "maior", 'n' para "menor", e 'i' para "igual").
O intervalo de possíveis números vai sendo ajustado com base nas dicas fornecidas pelo jogador e definido pelo mínimo (min) e máximo(max) em cada tentativa, permitindo que o computador dê um novo palpite aleatório dentro do intervalo já definido.
O jogo termina quando o jogador confirma que o palpite está correto ('i').
Para otimizar o processo, ajustei os limites mínimo e máximo do intervalo de possíveis números com base no feedback do jogador.
O computador faz um novo palpite dentro do intervalo ajustado, mantendo a aleatoriedade, mas restringindo as opções com o tempo.


Desafios e Dificuldades:

O controlo do intervalo de números no segundo jogo revelou-se um desafio, pois era importante garantir que o intervalo (min, max) não se tornasse inválido ou não gerasse um erro. Por exemplo, se o jogador der dicas incorretas (o jogador poderia dizer que o número é "maior" ou "menor" quando não há mais números no intervalo).
