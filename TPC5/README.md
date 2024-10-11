Este código é um sistema simples de gestão de um cinema, onde salas de cinema e filmes em exibição são armazenados, e ações como listar filmes, 
verificar disponibilidade de lugares e vender bilhetes podem ser realizadas. Cada sala de cinema é representada como um tuplo contendo o número de lugares 
disponíveis, uma lista de lugares vendidos, e o nome do filme em exibição.


Funcionalidades:
Listagem de Filmes: A função listarCinema exibe todos os filmes em exibição.

Verificação de Disponibilidade de Lugar: A função disponivel verifica se um lugar específico está disponível para um determinado filme.

Venda de Bilhete: A função vendeBilhete adiciona um lugar à lista de vendidos para um determinado filme.

Listagem de Disponibilidades: A função listarDisponibilidades mostra o número de lugares disponíveis para cada filme.

Inserção de Salas: A função inserirSala adiciona uma nova sala ao cinema, verificando se já não existe uma sala com o mesmo filme em exibição.

Menu Interativo: O menu implementa um loop interativo que permite ao utilizador realizar operações como criar sessões, listar filmes, verificar 
disponibilidade de lugares e vender bilhetes.


Desafios e Dificuldades Superadas:
Estrutura de Dados: Usar tuplos para representar as salas, e listas para armazenar os lugares vendidos, facilita a gestao de dados, mas requer atenção
ao manipular os índices corretamente.

Lógica de Disponibilidade: A função disponivel foi desenhada para verificar corretamente se um lugar está livre antes de vender o bilhete, evitando 
sobreposição de vendas.

Interface de Menu: A implementação do menu com um loop de interação melhora a usabilidade, mas pode ser desafiadora para garantir que o programa funcione 
corretamente com diferentes entradas do usuário.

Atualização de Dados: A necessidade de atualizar o estado do cinema (como a lista de filmes ou lugares vendidos) de forma correta após cada operação 
foi uma preocupação superada com a organização das funções.