# DDL - Linguagem de Definição de Dados
DDL (Data Definition Language). É utilizado para definir e excluir tabelas, os tipos de dados que nela serão armazenados e adicionar novas colunas as tabelas existentes. Os comandos que realizam essas funções são:

| Comando SQL | Descrição                                 |
| ----------- | ----------------------------------------- |
| CREATE      | Cria um objeto (Tabela, View, etc)        |
| ALTER       | Adiciona uma coluna a um objeto existente |
| DROP        | Deleta um objeto                          | 

## Criando tabelas
### Tipos de dados mais usados (Data types)
Para criar tabelas, cada coluna apresenta um tipo de dado, os principais são:
- **INT** - Numeros inteiros
- **DECIMAL(M, N)** - Numeros decimais
- **VARCHAR(1)** - String de um texto de tamanho 1
- **BOLB** - Binary Larg Object, Armazena dados grandes
- **DATE** - 'YYYY-MM-DD'
- **TIMESTAMP** - 'YYYY-mm-dd HH:MM:SS' - Usado para gravar quando algo acontece

Criar uma tabela usamos o comando "CREATE TABLE" e definimos os tipos de dados que cada coluna armazenará:
```sql
CREATE TABLE student (						 # cria tabela "student"
		student_id INT PRIMARY KEY,      # cria coluna "student_id" do tipo INT como sendo a chave primaria
		name VARCHAR(20),					   # cria coluna "name" do tipo VARCHAR com tamanho 20
		major VARCHAR(20)						# cria coluna "major" do tipo VARCHAR com tamanho 20
);
```

**Output table**

| student_id* | name        | major       |
| ----------- | ----------- | ----------- |
| INT PK      | VARCHAR(20) | VARCHAR(20) |

Outros comando utilizados na criação de tabelas:
```sql
CREATE TABLE student (									  # cria tabela "student"
        student_id INT  AUTO_INCREMENT,	 	   # cria coluna "student_id" do tipo INT e auto incrementa seu valor
        name VARCHAR(20) NOT NULL,		  		# cria coluna "name" do tipo VARCHAR com seu valor não podendo ser NULL
        major VARCHAR(20) UNIQUE,			       # cria coluna "major" do tipo VARCHAR com seu valor unico em toda tabela
		cpf VARCHAR(11) DEFAULT 'Unspecified', # cria colona "cpf" do tipo VARCHAR, se o valor não for especificado o valor padrão será "Unspecified"
		PRIMARY KEY(student_id) 				          # transforma a coluna "student_id" na chave primaria
);
```

## Gerindo tabelas existentes
Visualiza as informações da tabela student:
```sql
DESCRIBE student;
```

Deleta a tabela student:
```sql
DROP TABLE student;
```

Altera a tabela student adicionando a coluna "gpa" de tipo DECIMAL:
```sql
ALTER TABLE student ADD gpa DECIMAL(3, 2);
```

**Output table**

| student_id* | name        | major       | gpa           |
| ----------- | ----------- | ----------- | ------------- |
| INT PK      | VARCHAR(20) | VARCHAR(20) | DECIMAL(3, 2) | 

Altera a tabela student deletando a coluna "gpa":
```sql
ALTER TABLE student DROP COLUMN gpa;
```

# Tags
#sql #bancodedados 
# Veja Também
- [[SQL]]
- [[Banco de Dados]]
- [[SQL Queries]]