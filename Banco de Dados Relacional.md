# Banco de Dados Relacional ([[SQL]])
Banco de dados relacional é o tipo mais utilizado de banco de dados, é baseado em um esquema de tabelas que se relacionam umas com as outras, guardando dados relevantes.
Nesse modelo cada linha de uma tabela é uma entidade e cada coluna é um atributo dessas entidades.

## Relational Databese Management Systems (RDBMS)
São os programas que ajudam na gestão dos bancos de dados, trazendo uma interface de usuário, tirando a dependencia da linha de comando. 
Os principais programas RDBMS são:
	- MySQL, Oracle, postgreSQL, mariaDB, etc.
	
## Exemplos de Banco de Dados Relacional
### Tabela de Estudante

| ID  | Aluno  | Graduação  |
|:---:|:------:|:----------:|
|  1  |  Jack  |  Biologia  |
|  2  |  Kate  | Sociologia |
|  3  | Claire |   Ingês    |
|  4  |  John  |  Quimica   |

### Tabela do Usuário
|  Username  |  Senha   | Email |
|:----------:|:--------:|:-----:|
|  jsmith22  | wordpass |  ...  |
| catlover45 | apple223 |  ...  |
|  gamerkid  |   ...    |  ...  |
|  giraffe   |   ...    |  ...  |

As colunas "ID" e "Username" são as chaves unicas que identificam cada linha da tabela, são as **Chaves primarias ou Primary Key(PK)**

### Trabalhadores
| cpf    | nome   | sexo | salario | branch_id |
| ------ | ------ | ---- | ------- |:---------:|
| 445522 | Marcos | M    | 14000   |     1     |
| 442299 | Joao   | M    | 25000   |     2     |
| 885522 | Maria  | F    | 15000   |     3     |

Nesse caso a **PK** dessa tabela é o cpf de cada tabalhador, PKs que possuem um proposito no mundo real são chamadas de **Chave natural ou natural key**

### Branch
| branch_id | branch_nome | mgr_id |
| --------- | ----------- | ------ |
| 2         | Scranton    | 101    |
| 3         | Stamford    | 102    |
| 1         | Corporate   | 108    | 

A PK da tabela Branch está como uma **Chave Estrangeira ou Foreign Key(FK)** na tabela Trabalhadores.
FK são usadas para criar relações entre tabelas.

### Fornecedor das Branch
| branch_id | nome_fornecedor | tipo_suprimentos      |
| --------- | --------------- | --------------------- |
| 2         | Hammer Mill     | Papel                 |
| 2         | Uni-ball        | Utencilios de escrita |
| 3         | Patriot Paper   | Papel                 | 

branch_id e nome_fornecedor são as PKs dessa tabela, separadas elas não deixam cada linha unica, apenas juntas conseguem. É chamado de **Chave Primaria Composta ou Composite Primary Key(CPK)**.

# Tags
#sql #bancodedados 
# Veja Também
- [[SQL]]
- [[Banco de Dados]]
- [[Banco de Dados não relacional]]