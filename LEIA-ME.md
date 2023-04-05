Sistema de CRUD com Back-end feito em java com persistência dos dados em banco de dados MYSQL.

Versão utilizada: JavaSE-1.8

Usuário e Padrão são: ADMIN / SENHA123



Principal = Este código é um sistema básico de gerenciamento de jogadores de futebol em que um usuário pode:
inserir, alterar, excluir e listar jogadores, adicionar clubes e horários.
O sistema solicita credenciais de login para acessar o banco de dados MySQL e, em seguida, apresenta um menu interativo para permitir ao usuário selecionar as operações
desejados. Foi usado o "for each" que é uma forma mais simples de abranger uma coleção de elementos, especialmente para coleções de tamanho fixo, como arrays.



ClubeDAO = implementa um DAO para a entidade Clube, fornecendo métodos para salvar e recuperar objetos Clube do banco de dados.
O método salvar insere um novo objeto Clube no banco de dados e o método recuperar consulta o banco de dados para obter todos os objetos Clube armazenados,
e armazena em um ArrayList e retornando, a classe usa JDBC para interagir com o banco de dados.



TimeDAO = Funciona para manipulação de dados relacionados a times em um banco de dados.
A classe possui dois métodos: salvar e recuperar.
O método salvar insere um novo registro de tempo no banco de dados com base em um objeto Time passado como parâmetro
O método recuperar faz uma consulta ao banco de dados e retorna uma lista de objetos Time com os dados de todos os registros de times armazenados no banco de dados.



Clube, Jogador, Time e Login = , as classes possuem getters e setters para cada atributo, permitindo que os valores sejam acessados ​​e definidos de fora da classe.
