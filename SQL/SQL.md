# Structured Query Language (SQL)

SQL é uma linguagem padronizada para a interação com [[Banco de Dados Relacional]], com ela podemos interagir com o RDBMS para:
- Criar, recuperar, atualizar e deletar dados.
- Criar e gerir Banco de Dados.
- Criar templates para tabelas do BD.
- Fazer tarefas administrativas (Segurança, gerenciamento de usuários, importar/exportar, etc.).

OBS: Código SQL em um RDBMS nem sempre é compatível com outro sem necessidade de modificar o código.

## [[SQL Queries]]
Uma Query é um conjunto de instruções dadas ao RDBMS (Escrita em [[SQL]]) que fala para o RDBMS quais informações você quer que ele te dê.

O SQL é dividido em subconjuntos de acordo com as operações que queremos efetuar sobre um banco de dados:

## [[DML - SQL]]
DML (Data Manipulation Language). É utilizado para realizar inclusões, consultas, alterações e exclusões de dados presentes nas tabelas. Os comandos que realizam essas funções são:

| Comando SQL | Descrição                                            |
| ----------- | ---------------------------------------------------- |
| INSERT      | Inserir um registro em uma tabela                    |
| UPDATE      | Mudar os valores de dados em uma tabela já existente |
| DELETE      | Remover linhas existentes da uma tabela              | 

## [[DDL - SQL]]
DDL (Data Definition Language). É utilizado para definir e excluir tabelas, os tipos de dados que nela serão armazenados e adicionar novas colunas as tabelas existentes. Os comandos que realizam essas funções são:

| Comando SQL | Descrição                                 |
| ----------- | ----------------------------------------- |
| CREATE      | Cria um objeto (Tabela, View, etc)        |
| ALTER       | Adiciona uma coluna a um objeto existente |
| DROP        | Deleta um objeto                          | 

## [[DCL - SQL]]
DCl (Data Control Language). Controla os aspectos de autorização de acesso e manipulação dos dados dentro do banco de dados. Os comando que realizam essas funções são:

| Comando SQL | Descrição                                                         |
| ----------- | ----------------------------------------------------------------- |
| GRANT       | Autoriza o usuario executar operações                             |
| REVOKE      | Remove ou restringe a capacidade do usuario de executar operações | 

## [[DTL - SQL]]
DTL (Data Transaction Language). É utilizado para escrever permanentemente ou reverter as transações feitas. Os comando que realizam essas funções são:

| Comando SQL | Descrição                                       |
| ----------- | ----------------------------------------------- |
| BEGIN WORK  | Marca o começo de uma transação                 |
| COMMIT      | Finaliza uma transação                          |
| ROLLBACK    | Desfaz as mudanças feitas desde o ultimo COMMIT | 

## [[DQL - SQL]]
DQL (Data Query Language). É utilizado para fazer consultas dentro do banco de dados. Os comando que realizam essas funções são:

| Comando SQL | Descrição                                               |
| ----------- | ------------------------------------------------------- |
| SELECT      | Seleciona e mostra as colunas das tabelas especificadas | 

# Tags
#sql #bancodedados