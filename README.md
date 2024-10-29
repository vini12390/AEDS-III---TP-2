Integrantes: Vinícius Figueiredo e Arthur Crossy
Descrição Geral
Esta aplicação tem como objetivo registrar dados em um arquivo externo, armazenando informações como nome, data de criação, data de conclusão, status e prioridade de cada registro. Os dados são persistidos em um formato estruturado para facilitar a leitura e análise posterior.
Ademais foram acrescidos: O envolvimento e a criação e manipulação de entidades de tarefas e categorias, utilizando técnicas avançadas de estrutura de dados, como a Árvore B+ para implementar índices e relacionamentos.

Funcionalidades
Criação de registros: Permite adicionar novos registros ao sistema, definindo os atributos nome, data de criação, status e prioridade. A data de conclusão é inicializada como nula e pode ser atualizada posteriormente.
Leitura de registros: Carrega os registros existentes do arquivo para a memória, permitindo a visualização e manipulação dos dados.
Atualização de registros: Permite modificar os atributos de um registro existente, como status ou data de conclusão.
Remoção de registros: Permite excluir registros indesejados do sistema.
Persistência de dados: Salva as alterações realizadas nos registros no arquivo externo de forma persistente.

Tecnologias Utilizadas
Linguagem de programação: Java

Classes criadas no TP2: 

Classe ArquivoCategoria

ela constroi o arquivo de categorias, e tem seu CRUD de categorias implementado.

Classe ArquivoTarefa

ela constroi o arquivo de tarefas, e tem seu CRUD de tarefas implementado.

Classe ArvoreBMais

estrutura árvore b+ implementada.

Classe Categoria

objeto do tipo categoria implementado para ser usado, com seus sets/gets/métodos de serialização em um array de bytes.

Classe ControleCategorias

Classe que possui métodos que interagem com as categorias(mostraCategorias) conforme as requisições do menu provenientes do usuário.

Classe ControleTarefas

Classe que possui métodos que interagem com as tarefas(buscarTarefas e mostrarTarefas) conforme as requisições do menu provenientes do usuário.

Classe MenuCategoria

Classe que constroi o menu das categorias, que possui o método incluirCategoria implantado.

Classe MenuTarefas

Classe que constroi o menu das tarefas, que possui o método incluirTarefa implantado.

Classe ParCategoriaTarefa

Clases que implementa o par Categoria-Tarefa, um relacionamento.

Classe ParNomeID

Classe que implementa o índice indireto ParNomeID, que possui método clone, compareTo, toString, size e métodos de serialização em um array de bytes.

além disso, são implementados também as interfaces novas:

RegistroArvoreBMais

interface que possui os métodos de serialização em array de bytes, compareTo, clone, e size, que são utilizados nos registros com a árvore b+.
