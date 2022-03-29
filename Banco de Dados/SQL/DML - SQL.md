# DML - Linguagem de Manipulação de Dados
DML (Data Manipulation Language). É utilizado para realizar inclusões, consultas, alterações e exclusões de dados presentes nas tabelas. Os comandos que realizam essas funções são:

| Comando SQL | Descrição                                            |
| ----------- | ---------------------------------------------------- |
| INSERT      | Inserir um registro em uma tabela                    |
| UPDATE      | Mudar os valores de dados em uma tabela já existente |
| DELETE      | Remover linhas existentes da uma tabela              | 

## Manipulando dados
### Inserir dados em uma tabela
Adiciona uma linha na tabela student com os valores "1", "Jack" e "Biology" de acordo com a ordem que as colunas foram criadas:
```sql
INSERT INTO student VALUES(1, 'jack', 'Biology');
```

Adiciona uma linha na tabela student com os valores "2" e "Bia" respectivamente nas colunas especificadas. Colunas que não forem especificadas retornarão valor "NULL":
```sql
INSERT INTO student(student_id, name) VALUES(2, 'Bia');
```

### Atualizando e deletando
Atualiza as linhas onde a coluna "major" é igual a "Bio" para "Biology":
```sql
UPDATE student
SET major = 'Biochemistry'
WHERE major = 'Bio';
```

Atualiza as linhas onde a coluna "major" é igual a "Bio" **OU** "Chemestry" para "Biochemistry":
```sql
UPDATE student
SET major = 'Biochemistry'
WHERE major = 'Bio' OR major = 'Chemestry';
```

Deleta as linhas da tabela "student" onde a coluna "name" for igual a "Maria":
```sql
DELETE FROM student
WHERE name = 'Maria';
```

"WHERE major **Comparação** 'Bio' " lista de operadores de comparação:
- **=** - igual a
- **<>** - diferente de
- **<** - menor que
- **>** - maior que
- **<=** - menor ou igual a
- **>=** - maior ou igual a

# Tags
#sql #bancodedados 
# Veja Também
- [[SQL]]
- [[Banco de Dados]]
- [[SQL Queries]]