# Sistemas de Backup
Backup é a tarefa de manter uma cópia de segurança de um conjunto de dados em um lugar geograficamente diferente do original. Existem diversos sistemas de backup que facilitam e automatizam essa tarefa.

- Flag Archive: Valor booleano presente no arquivo que determina se ele foi modificado ou não, assim dizendo se necessita de um novo backup ou não.

Não há um padrão de tempo de backup, depende da frequência em que a organização altera os dados, virando de organização para organização.

## Tipos de backup
### Backup completo
- Todos os dados são salvos em uma única cópia de segurança.
	- Execução do Backup: demorado
	- Restauração: demorada
	- Apaga o flag archive
	- Feito periodicamente e com menor frequência
	- Primeiro a ser executado em um sistema que nuca foi feito seu backup.

### Backup incremental
- Cópia dos dados que **contém o flag archive**
- Comparados com o último backup
	- Execução do Backup: rápido
	- Restauração: demorada, pois necessita de todos os backups anteriores
	- Apaga o atributo de marcação

### Backup diferencial
- Cópia dos dados que contém o atributo de marcação, comparado-os com o último backup completo ou incremental.
	- Execução do Backup: Mais rápido que o completo, e mais lento que o incremental
	- Restauração: Maśi rápido que ambos
	- NÃO apaga o atributo de marcação

### Backup de cópia
Cópia comum de todos os dados, utilizado de ultima hora para, por exemplo, efetuar uma manutenção no sistema.

### Backup diário
Consiste em copiar todos os arquivos modificados ou criados na execução do backup.
![](https://i.imgur.com/fYfvcBl.png)


# Tags
#hardware #computador #arquiteturadecomputação 
# Veja Também
- [[Sistema de Armazenamento (Memórias)]]
- [[Sistemas de Computação]]