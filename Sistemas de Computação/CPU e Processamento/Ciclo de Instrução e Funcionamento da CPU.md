# Ciclo de Instrução e Funcionamento da CPU
Para se construir uma CPU, a única função que deve ser implementada é a que busque a instrução correta na memória, decodifique-a e a execute, passando em seguida para a próxima instrução. Esse "algoritmo do funcionamento da CPU", ou princípio de funcionamento, é chamado de **ciclo de instrução**.

A versão simplificada do ciclo de instrução da CPU é:
- Ínicio
- **Buscar a próxima instrução**
- Interpretar a Instrução
- Executar a isntrução
- **Buscar a próxima instrução**
- Término

Primeiro é necessário identificar onde na memória está a instrução, em seguida trazer o conteúdo do endereço para a CPU:
- Cálculo do endereço da instrução
	- O registrador contador de programa é copiado para o registrador de endereço da memória
- Busca da instrução
	- A unidade de controle gera o sinal de leitura e o conteúdo da posição solicitada é transmitido para a CPU, chegando no registrador de dados da memória. A instrução é então copiada para o registrador da instrução
	
Uma vez a isntrução armazenadano registrador de instrução, é possivel executar a etapa da:
- Decodificação da instrução
	- A unidade de controle decodifica a instrução (código de operação) armazenada no registrador de isntrução e passa a gerar os sinais de controle na orde, necessária para concluir a operação

Assim, a CPU sabe o que deve ser feito. Podendo prosseguir com:
- Cálculo dos endereços dos operandos:
	- Verifica onde está os operandos das instruções.
- Busca dos operandos:
	- vai até a posição de memória, registrador, ou periférico, e copia os dados do operando para o local adequado.
- Execução da operação:
	- de posso do código de operação e dos operandos é possível executar a instrução, etapa que ocorre geralmente na ULA
- Cálculo dos endereços dos resultados:
	- Verifica onde podem ser armazenados os resultador
- Armazenamento dos resultador
	- Escreve os resultador nos locais adequados
	- Se o contador de programa não tiver sido modificado nesta etapa, ele é incrementado para prosseguir para a próxima instrução.

Muitas vezes o ciclo de instrução é representado em cinco etapas, forma comumente adotada para a implementação da [[Pipeline da CPU]] de instruções:
- Busca da instrução (Instruction Fetch)
- Decodificação da instrução
- Busca do(s) operando(s)
- Execução da instrução
- Armazenamento do(s) resultado(s).

# Tags
#hardware #computador #arquiteturadecomputação 
# Veja Também
- [[Sistemas de Computação]]
- [[Pipeline da CPU]]
- [[Unidade Central de Processamento (CPU)]]
- [[Arquitetura do Conjunto de Instruções (ISA)]]