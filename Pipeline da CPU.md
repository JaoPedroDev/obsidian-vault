# Pipeline da CPU
Antigamente, as instruções executadas na [[Unidade Central de Processamento (CPU)]] eram feitas de maneira sequencial, ou seja, uma instrução de cada vez, essa sendo uma tecnica que disperdissava tempo. Assim, foi empregado na CPU o modelo de "linha de montagem" das fabricas, dividindo a execução de cada instrução em etapas, chamado de pipeline, com isso o tempo ocioso da CPU foi diminuido.

Antigo modelo de execução (Sequencial):
![](https://i.imgur.com/eznpNr0.png)

No modelo de execução de pipeline, as instruções são divididas em estágios e inseridas de modo que as instruções fiquem parcialmente sobrepostas na execução. Diminuindo muito o tempo ocioso da CPU.

Novo modelo de execução (Pipeline):
![](https://i.imgur.com/oTaholG.png)

No exemplo, no modelo de pipeline foram executadas 6 instruções e inseridas trechos de outras 4 instruções no mesmo tempo de execução do modelo antigo.

Os estágios apresentados nos exemplos são:
- BI - Busca da Instrução
- DI - Decodificação da Instrução
- BO - Busca do(s) Operando(s)
- EI - Execução da Instrução
- AR - Armazenamento do(s) resultado(s)

Esses estágios da pipeline sempre possuem a mesma duração, ajustada pelo que leva mais tempo. A qauntida de estágios depende da fabricação de cada CPU.

## Os Três Tipos de Conflitos
Na pipeline, as instruções são carregadas sequencialmente, pressupondo que a ordem das instruções na memória será seguida à risca. Mas nem sempre isso ocorre.

Há problemas que ocorrem na "linha de montagem" as vezes, algumas da vezes até precisando reiniciar completamente essa linha.

Esses problemas que atrasam a execução são chamados de **conflitos (hazards)** e o atraso gerado para resolver esses coflitos é chamado de **pipeline stall**.

### Conflito de desvio, ou de controle
Ocorre quando há um pedido de interrupção/desvio condicional. Assim os estágios que foram executados antes do devio são descartados para reiniciar a pipeline.
![](https://i.imgur.com/a0TVPoS.png)

### Conflito de dados
Quando o dado que precis ser manipulado por um instrução é o produto de uma instrução que ainda está em execução.
Então ess instução que requer o dado é atrasada esperando a outra instrução ser terminada.
![](https://i.imgur.com/RL9Q8Qp.png)

### Conflito estrutural
Similar ao conflito de dados, é o componente requerido para a execução de um determinado estágio que está ocupado. Ex: enquanto uma instrução busca um operando na memória principal, o estágio de busca da instrução da pipeline não pode ser executado e precisa aguardar.

# Tags
#hardware #computador #cpu 
# Veja Também
- [[Ciclo de Instrução e Funcionamento da CPU]]
- [[Unidade Central de Processamento (CPU)]]
- [[Sistemas de Computação]]