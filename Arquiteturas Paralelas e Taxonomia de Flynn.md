# Arquiteturas Paralelas e Taxonomia de Flynn
A computação paralela é caracterizada pelo uso de várias unidades de processamento ou processadores para executar uma computação de forma mais rápida. É baseada no fato de que o processo de resolução de um problema pode ser dividido em tarefas menores, realizadas simultaneamente por meio de algum tipo de coordenação. Conceito originalmente introduzido no CDC (Control Data Corporation) em 1964. 

## Taxonomia de Flynn
Os modelos de computação paralela existentes, conforme Michael J. Flynn estabeleceu, são:

- **SISD (Single Instruction, Single Data)**: As instruções organizadas de maneira sequencial, mas podem ser executadas de forma sobreposta em diferentes estágios (pipelining).
- **SIMD (Single Instruction, Multiple Data)**: Vários dados são processados no comando de apenas uma instrução. Utiliza-se uma organização de memória em diversos módulos.
- **MISD (Multiple Instruction, Single Data)**: Um conjunto de dados é colocado concorrente em múltiplas unidades de processamento. Cada UP opera de maneira independente via conjuntos independentes de instruções.
- **MIMD (Multiple Instruction, Multiple Data)**: Processamento de múltiplos dados por parte de múltiplas instruções. Neste caso há várias unidades funcionais.

## Multiprocessador Simétrico (SMP)
Conhecidos como arquiteturas de compartilhamento total, que são caracterizadas por até dezenas de processadores compartilhando os mesmos recursos computacionais e rodando um único sistema operacional. São simétricos pois compartilhamd os mesmos custos para acesso à memória principal.

Os processadores multicore se encaixam nessa subcategoria dos sistemas MIMD.

## Cluster
É um conjunto de computadores ligados através de uma rede e se comportam como um unico computador para realizar os processamentos.

# Tags
#hardware #computador #cpu 
# Veja Também
- [[Processadores Superescalares]]
- [[Unidade Central de Processamento (CPU)]]
- [[Sistemas de Computação]]
- [[Computação Distribuída]]