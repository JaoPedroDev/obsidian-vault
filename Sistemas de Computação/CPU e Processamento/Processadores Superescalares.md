# Processadore Superescalares
A idéia geral do paralelismo em nível de instrução, ou Instruction Level Parallelism (ILP), é que algumas instruções de um programa poderiam ser executadas em paralelo, sem prejuízo para o resultado final.

Para o funcionamento dessa idéia é necessário emitir, ou despachar, mais de uma isntrução por ver para execução na CPU, cada um em sua pipeline, técnica conhecida como **despacho múltiplo (multiple issue)**.

O despacho múltiplo possui duas vertentes:
- Despacho Múltiplo Estático: A otimização das instruções para funcionarem em paralelo devem ser explicitas no código do programa.
- Despacho Múltiplo Dinãmico: A otimização das intruções para funcionarem em paralelo é feita pelo próprio hardware no momento de sua execução. São chamados esses processadores de **superescalares**.

Um processador superescalar possui várias **unidades funcionais** que são usadas para o paralelismo, cada unidade pode executar uma instrução de maneira independente. As unidades mais comuns:
- Unidade de inteiros (ULA)
- Unidade de ponto flutuante (FPU)
- Unidade de cálculo vetorial
- Unidade de carga
- Unidade de armazenamento

A figura a seguir ilustra o funcionamento de um processador superescalar básico. Observe o paralelismo nas unidades funcionais, que correspondem ao estágio de execução da operação da pipeline.
![](https://i.imgur.com/fDX0g3X.png)

As implementações superescalares utilizam , na prática, três técnicas juntas: emprego de múltiplas unidades funcionais, execução fora de ordem e renomeação de registradores.

## Simultaneous Multithreading (SMT)
Além do paralelismo empregado nas sequências de instruções, há também o paralelismo entre multiplas aplicações, ou seja, mais de um programa, ou diferentes partes de um mesmo programa, sendo executados ao mesmo tempo. Isso é chamado de **Simultaneous Multithreading(SMT)** (Hyperthreading para a Intel).

Algumas sequências de instruções não utilizam completamente o paralelismo disponivel nas unidades funcionais, disperdiçando recursos, com isso a técnica SMT pode aproveitar os recursos execedentes com isntruções de outra thread. Para isso é necessário um conjunto de registradores de controlre e de estado para cada thread.

# Tags
#hardware #cpu #arquiteturadecomputação 
# Veja Também
- [[Conjunto Reduzido de Instruções (RISC)]]
- [[Pipeline da CPU]]
- [[Ciclo de Instrução e Funcionamento da CPU]]