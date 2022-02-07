# Unidade Central de Processamento(CPU)
Um programa para ser executado por uma CPU, deve ser contituido por uma série de instruções (em linguagem de máquina) armazenadas em posições sucessivas da memória principal, sendo a execução sequencial dessas instruções.

Cada instrução atuará sobre um ou mais dados que são o(s) **operando(s)** da instrução, gerando um respectivo resultado que será armazenado na memória.
Ex: Soma - operando_1 + operando_2 = resultado

O [[Ciclo de Instrução e Funcionamento da CPU]] é conhecida como ciclo de busca e execução de instruções, ou **busca - decodificação - execução** de instruções.

-> ÍNICIO
**-> Busca a próxima instrução**
-> Interpreta a instrução (decodificação)
-> Executa a instrução
**-> Busca a próxima instrução**
-> TÉRMINO.

## Funções de processamento: 
A **Unidade Lógica Aritimética(ULA)** se encarrega de realizar as atividades relacionadas com a efetiva excução das operações, sendo encarregada de realizar as operações de aritméticas e lógicas.

Atualmente, os microprocessadores possuem mais de uma unidade lógica além da ULA, como a FPU(Float Point Unit), que é especializada em calculos de ponto flutuante. Alguns processadores possuem até mesmo unidades especializadas em calculos para criptografia. Essas unidades são genericamente chamas de **Unidades Funcionais**.

## Funções de controle:
A **Unidade de Controle(UC)** se encarrega das atividades de busca, interpretação e controle da execução das instruções, bem como do controle da ação dos demais componentes do sistema de computação (memória, entrada/saída), ou seja, é encarregada de controlar as demais unidades e, por extensão, todo o computador.

A unidade de controle pode ser implementada como uma máquina de estados finitos (FSM - Finite State Machine), ou de uma forma mais sofisticada, através de microprogramação, onde as instruções de máquina são subdivididas em partes ainda mais básicas.

## Tarefas de processamento de dados
Dentre as tarefas de processamento de dados podem ser citadas:
-   Operações aritméticas: soma, subtração, multiplicação e divisão;
-   Operações lógicas: and, or, xor, not;
-   Movimentação de dados: memória – CPU (registrador), CPU (registrador) – memória, registrador – registrador;
-   Desvios: alteração da sequência de execução das instruções;
-   Operações de entrada ou saída.

## Desempenho computacional
É medido o desempenho de um computador através de quão rápido ele processa dados ou transfere grandes volumes de dados. Dentre os parâmetros ligados à CPU podemos destacar o MIPS (Milhões de Instruções por Segundo) e o FLOPS (Instruções de Ponto Flutuante por Segundo).

## Registradores
São circuitos formados por flip-flops, dedicados ao armazenametno de uma palavra de dados. Seu controle é feito pela Unidade de Controle.

Existem dois tipos de registradores, classificados como:
- Registradores visíveis ao usuário: São resgistradores que podem ser manipulados por programas, são de proprosito geral.
- Registradores de controle e de estado: São registradores utilizados pela unidade de controle e pelo Sistema Operacional.

### Organização dos Registradores
Toda CPU necessita de um conjunto de registradores para seu funcionamento.

O modelo de Von Neumann estipula que o programa seja armazenado na memória. A CPU deve então buscar a instrução a ser executada, armazenála, decodifica-la e executa-la...

Temos então a necessidade de dois apres de registradores, um para a comunicação efetiva com a memória e outro pra o controle do programa:
- Contador de Programa(PC - Program Counter)
	- Armazena o endereço da memória principal onde está a próxima instrução a ser executada.
- Registrador de Instrução (IR - Instruction Register)
	- Armazena a instrução do programa que está sendo executada no ciclo de instrução atual
- Registrador de Endereços da Memória (MAR - Memory Adress Register)
	- Armaena o endereço a ser acessado na memória principal
- Registrador de Dados da Memória (MBR - Memory Buffer Register, ou MDR - Memory Data Register)
	- Armazena os dados contidos, ou a serem escritos, na posição de memória indicada pelo registrador de dendereços da memória

Outro par de registradores se faz necessário para que a ULA possa efetuar suas operações e armazenar os resultados. São eles:

- **Acumulador**
	- Armazena um dos operandos das operações a serem executadas na ULA e também os resultados dessas operações.
- **Registradores Auxiliares**
	- É preciso haver no mínimo um registrador auxiliar para armazenar o segundo operando a ser utilizado pela ULA, porém o mais comum é que haja uma quantidade um pouco maior desses registradores.

Toda vez que uma operação é realizada na ULA são gerados indicadores (**flags**), também chamados de **códigos de condição**. Esses códigos são bits "individuais" que trazem informações adicionais sobre as operações realizadas. Alguns dos códigos de condição mais comuns são:

- **Zero**
    - Indica se o resultado da operação foi zero (ou não)
- **Sinal**
	- Indica o sinal do resultado da operação (positivo ou negativo)
- **Carry** / Borrow
    - Indica se houve o transporte na operação aritmética. "Vai um" (carry) na adição, ou "empresta um" (borrow) na subtração.
- Estouro (**Overflow**)
    - Usado para indicar que o tamanho do resultado da operação é maior do que o tamanho da palavra. Por exemplo, na multiplicação de dois números muito grandes.
- Igualdade (**Equal**)
	- Indica se os operandos na ULA são iguais.

Os bits dos códigos de condição normalmente são agrupados em um registrador chamado de **Registrador de status (PSW - Program Status Word)**. Além disso, esse registrador também inclui indicadores referentes ao funcionamento geral da CPU:
- Modo supervisor (modo kernel)
	- usado para permitir que a CPU execute determinadas instruções privilegiadas.
- Habilitação e inibição de interrupções
	- Usado no tratamento de múltiplas interrupções
- Controle de frequência de clock
	- Usado para gerenciar o desempenho e o consumo de energia dos processadores

## Estrutura mínima de uma CPU
Para o funcionamento mínimo a CPU requer:
- O Barramento interno
- A ULA
- A Unidade de controle
- Ao menos sete registradores:
	- MAR
	- MBR
	- PC
	- IR
	- Acumulador
	- Registrador Auxiliar
	- PSW

A unidade de controle se conecta a todos os demais componentes e possui também algumas conexões externas:
- Sinal de controle de leitura, ou escrita na memória principal
- Entrada de interrupção (INT) externa
- Circuuitos de clocl (cristal e clock) para sincronizar o funcionamento da CPU e de todo o sistema computacional
# Tags
#hardware #cpu #arquiteturadecomputação 

# Veja Também
- [[Sistemas de Computação]]
- [[Arquitetura do Conjunto de Instruções (ISA)]]