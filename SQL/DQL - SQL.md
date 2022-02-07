# DQL - Linguagem de Consulta de Dados
DQL (Data Query Language). É utilizado para fazer consultas dentro do banco de dados. Os comando que realizam essas funções são:

| Comando SQL | Descrição                                               |
| ----------- | ------------------------------------------------------- |
| SELECT      | Seleciona e mostra as colunas das tabelas especificadas | 

## Solicitando dados
Seleciona todas as colunas da tabela "student":
```sql
SELECT * 
FROM student;
```

Seleciona as colunas "name" e "major" da tabela "student" e coloca em ordem alfabetica de acordo com as colunas "major" e "student_id" e retorna as 5 primeiras linhas:
```sql
SELECT name, major
FROM student
ORDER BY major, student_id
LIMIT 5;
```

Seleciona todas as colunas da tabela "student" e onde "major" é igual a "Art" **OU** "undecided":
```sql
SELECT *
FROM student
WHERE major = 'Art' OR major = 'undecided';
# alternativamente:
WHERE major IN ('Art', 'undecided');
```

# Tags
#sql #bancodedados 
# Veja Também
- [[SQL]]
- [[Banco de Dados]]
- [[SQL Queries]]