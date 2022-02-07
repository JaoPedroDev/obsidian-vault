# SQL Queries
## Queries
- Uma Query é um conjunto de instruções dadas ao RDBMS (Escrita em [[SQL]]) que fala para o RDBMS quais informações você quer que ele te dê.

```sql
SELECT employee.name, employee.age
FROM employee
WHERE employee.salary > 30000;
```

Esse bloco de codigo diz ao RDBMS selecionar as colunas *name* e *age* da tabela *employee* e retornar as linhas em que o *salary* for maior que 30000.
