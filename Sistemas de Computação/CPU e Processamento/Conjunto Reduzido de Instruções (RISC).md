# Computador com Conjunto Reduzido de Instruções (RISC)
No principio, o hardware que era o responsável por executar os softwares, ou seja, eram criados mais e mais instruções de maquinas para cada caso especifico de cada programa. 

Porém isso veio a ser um problema, pois não havia um padrão entre os processadores e era dificil o desenvolvimento de programas através de codigo de maquina. Com isso surgiu a arquitetura RISC (Reduced Intruction-Set Computer), utilizando apenas as instruções mais utilizadas e otimizadas, obtendo um maior desempenho global.

As principais caracteristicas dessa arquitetura são:
- As operações são feitas de registrador para registrador
- O acesso à memória é feito exclusivamente por instruções simples de carga e armazenamento (LOAD e STORE)
- Empregam-se apenas modos de endereçamento simples e eficientes
- Usam-se formatos de instruções simples. As instruções normalmente tem todas o mesmo tamanho
- Há um maior número de registradores disponiveis
- Enfoque na otimização da [[Pipeline da CPU]]
- As diferentes instruções possuem o mesmo tempo de execução

# Tags
#hardware #computador #cpu #arquiteturadecomputação 
# Veja Também
- [[Unidade Central de Processamento (CPU)]]
- [[Arquitetura do Conjunto de Instruções (ISA)]]
- [[Ciclo de Instrução e Funcionamento da CPU]]