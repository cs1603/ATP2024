Este projeto implementa um sistema de gestão de alunos em Python que permite criar, armazenar, consultar e manipular informações de alunos em turmas.
Cada aluno possui um nome, um identificador único (ID), e três notas: nota do Trabalho Prático Contínuo (TPC), nota do Projeto e nota do Teste. 
Esses dados são geridos dentro de uma turma, que é uma lista de alunos.

O sistema oferece um menu interativo que permite ao utilizador realizar várias operações, como criação de turmas, inserção de alunos, consulta e listagem, bem 
como salvar e carregar turmas a partir de arquivos.

Funcionalidades
Estrutura de Dados

O sistema utiliza uma estrutura simples:

Cada aluno é representado por um tuplo: (nome, id, [notaTPC, notaProj, notaTeste]).
Uma turma é uma lista de alunos, onde cada aluno é armazenado como uma tuplo.
Funcionalidade: Criar Aluno (criar_aluno)

Esta função recolhe os dados de um aluno, como nome, ID e as notas, a partir da entrada do utilizador. Ela retorna um tuplo com essas informações.

Funcionalidade: Criar Turma (criar_turma)

Esta função cria uma nova turma, que é uma lista vazia, e chama a função criar_aluno() repetidamente para adicionar alunos até que o utilizador decida parar.

Funcionalidade: Inserir Aluno (inserir_aluno)

A função inserir_aluno permite a inserção de um novo aluno numa turma existente, verificando antes se já existe um aluno com o mesmo ID, evitando duplicações.

Funcionalidade: Listar Turma (listar_turma)

Esta função percorre a lista de alunos (turma) e imprime as informações de cada aluno. Se a turma estiver vazia, o programa indica que não há alunos.

Funcionalidade: Consultar Aluno (consultar_aluno)

A função consultar_aluno permite ao utilizador procurar um aluno específico pelo seu ID e exibe as informações que lhe correspondem.

Funcionalidade: Guardar Turma em Ficheiro (guardar_turma)

Esta função permite salvar os dados da turma atual num ficheiro de texto. Cada aluno é escrito no ficheiro em formato de string.

Funcionalidade: Carregar Turma de Ficheiro (carregar_turma)

Permite carregar uma turma de um ficheiro de texto. O ficheiro é lido linha por linha, e os dados dos alunos são exibidos no terminal.

Menu Interativo

O menu interativo guia o utilizador através das várias opções disponíveis, permitindo realizar operações como criar uma turma, inserir alunos, listar a turma, 
consultar informações de um aluno, salvar a turma num ficheiro e carregar a turma a partir de um ficheiro. O ciclo principal do menu continua até que seja escolhida 
a opção "0".

Desafios Ultrapassados
Evitar Duplicados de IDs: Um dos principais desafios foi evitar a inserção de alunos com IDs duplicados. Para resolver isso, foi criada a função 
aluno_naoexiste que verifica se o ID do aluno já está presente na turma antes de inseri-lo.
Manipulação de Ficheiros: Outro desafio foi garantir que a turma pudesse ser salva e carregada corretamente a partir de um ficheiro. Isso foi resolvido 
utilizando a manipulação de ficheiros em Python (open, write, read). No entanto, um aprimoramento adicional seria serializar e deserializar os dados da turma 
usando formatos mais estruturados, como JSON.
Menu Interativo: A implementação de um menu interativo que permita realizar várias operações sequencialmente, sem sair do programa, foi outro desafio 
abordado com sucesso. Isso exigiu a criação de um loop while que só é encerrado quando o usuário escolhe a opção de sair (opção == '0').
Tratamento de Erros Simples: Adicionar verificações de erros básicos para garantir que, quando o usuário escolhe uma opção inválida, o programa o informe e 
continue a executar foi outro desafio. O tratamento foi implementado com uma cláusula else no final do loop principal.

Este projeto cumpre o objetivo de fornecer uma aplicação básica de gestão de alunos com funcionalidades de criação, consulta, armazenamento e 
recuperação de turmas. Embora seja uma solução inicial, há espaço para melhorias, 
especialmente em termos de validação de entradas e persistência de dados mais eficiente.