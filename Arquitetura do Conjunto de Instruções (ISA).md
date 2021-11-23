# Arquitetura do Conjunto de Instruções (ISA)
A Instruction Set Architecture (ISA) é a especificação do projeto da [[Unidade Central de Processamento (CPU)]], e se refere a quais instruções a CPU será capaz de executar. Ela define:
- O formato das instruções são fornecidas à CPU
- Quais registradores existem e podem ser manipulados à CPU
- Quais os operandos manipulados por essas instruções
- Todas as demais características necessárias para se escrever programas para a CPU

Essas instruções são as **Instruções de máquina**, carregadas na forma de códigos binários na memória do computador, conforme o modelo estabelecida por Von Neumann. Toda instrução é dividida em duas partes:
- Código de operação (opcode): O que deve ser feito. Ex: Soma, escrita de dados, etc.
- Operandos: Dados manipulados pela instrução
	- Operando fonte: Ex: Os números a serem somados.
	- Operando destino: Ex: Onde será armazenado o resultado da soma.

Usualmente representamos as instruções de máquina em uma linguagem mais legivel através de uma linguagem de baixo nível chamada **Assembly**.

## Tipos de Operandos
Os operandos podem ser basicamente:
- Endereços:
	- Registradores
	- Memória principal
	- Preiféricos
- Números:
	- Inteiros
	- Inteiros sinalizados
	- Decimais codificados em binário
	- Ponto flutuantes
- Caracteres:
	- Necessitam de um código para serem representados em binário. O mais utilizado é p ASCII
- Dados lógicos:
	- Variáveis booleanas

## Tipos de Instruções
Todo ISA possui instruções que permitam que o computador cumpra suas funções básicas:
- Processar dados:
	- Intruções lógicas: XOR (OU Exclusivo), AND (E), OR (OU) e NOT (NÃO)
	- Intruções aritméticas: As quatro operações fundamentais
- Armazenar e Comunicar dados:
	- Intruções de movimentação de dados
	- Intruções de carga e armazenamento
	- Intruções de entrada e saída
- Exercer controle (sobre o fluxo de execução das instruções):
	- Intruções de controle:
		- Desvios incondicionais: Desvio imediato para o endereço de memória especificado, usada no final de um laço para provocar sua repetição
		- Desvios condicionais: Se a condição especidficada for verdadeira, desvia para o endereço de memória especificado
		- Chamadas de sub-rotinas: Intrução CALL para chamar a sub-rotina e RETURN para retornar ao programa principal

## Modos de Endereçamento
Os Modos de Endereçamento envia à CPU o operando a ser usado para uma instrução específica.
Há sete modos de endereçamento básicos:
- Imediato: O operando da instrução é o valor a ser somado
- Direto: O Operando da isntrução é o endereço da memória que contém o valor a ser somado
- Indireto: É feita uma operação em 2 etapas. O endereço indicado pela instrução contém o endereço de onde está o operando
- Registrador: O operando da instrução está armazenado no registrador indicado
- Indireto via Registrador: É feita uma operação em 2 etapas. O registrador indicado na instrução contém o endereço da memória onde está o operando
- Indexado: É utilizado no gerenciamento da memória pelo sistema operacional, control de laços e operações iterativas
- Stack: É utilizado para manipular operandos que se encontrem na stack da memória.

## O Projeto de uma ISA
Para projetar uma ISA deve-se penser em:
- Quantos bits para a arquitetura
	- 8, 16, 32 ou 64 bits
- Quais tipos de operandos que serão suportados
	- Ponto flutuante requer instruções aritiméticas específicas para ele
	- Mais de um código de caracteres requer instruções de conversão de um formato para outro
- Quais intruções estarão disponìveis
	- A quantidade e a complexidade das instruções terão impacto profundo na implementação dos microprocessadores
- Modos de Endereçamento e Registradores
	- Quais modos estarão disponiveis, quais deles serão privilegiados
	- Quantos registradores estarão disponiveis, as operações serão focadas na memória, ou no uso dos registradores.

## Computador com Conjunto Reduzido de Instruções (RISC)
No principio, o hardware que era o responsavel por executar os softwares, ou seja, eram criados mais e mais instruções de maquinas para cada caso especifico de cada programa. 

Porém isso veio a ser um problema, pois não havia um padrão entre os processadores e era dificil o desenvolvimento de programas através de codigo de maquina. Com isso surgiu a arquitetura RISC (Reduced Intruction-Set Computer), utilizando apenas as instruções mais utilizadas e otimizadas, obtendo um maior desempenho global.

As principais caracteristicas dessa arquitetura são:
- As operações são feitas de registrador para registrador
- O acesso à memória é feito exclusivamente por instruções simples de carga e armazenamento (LOAD e STORE)
- Empregam-se apenas modos de endereçamento simples e eficientes
- Usam-se formatos de instruções simples. As instruções normalmente tem todas o mesmo tamanho
- Há um maior número de registradores disponiveis
- Enfoque na otimização da pipeline de instruções
- As diferentes instruções possuem o mesmo tempo de execução


# Tags
#hardware #computador #cpu #linguagemdeprogramacao
# Veja Também
- [[Sistemas de Computação]]
- [[Unidade Central de Processamento (CPU)]]