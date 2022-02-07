# Barramento (Bus)
São os conectores dos componentes de um computador que funcionam em um determinado padrão.
Ex: entrada para placa de vídeo, memória ram, cabos de memória, USB, etc.

Todo barramento carrega três tipos de informação:
- Dados a serem lidos ou escritos.
- Endereço: a posição (endereço de emória E/S) onde a informação será lida ou escrita.
- Controle: Série de sinais digitais (bits) de controle para a efetivação das operações de leitura e escrita.

## Características dos Barramentos
- Sincronização:
	- Síncrono - o barramento utiliza o clock para sincronizar as transferências de informação.
	- Assíncrono - não utiliza o clock.
- Compartilhamento:
	- Multiplexado - as linhas do barramento são compartilhadas entre diversos dispositivos, ou funções.
	- Dedicado - as linhas são exclusivas para suas funções e dispositivos.
- Tipo de transmissão:
	- Paralelo - os bits de dados são transmitidos ao mesmo tempo, cada um em sua linha.
	- Seriaç - os bits de dados são transmitidos um após o outro em uma única linha.
- Largura do barramento: 
	- Largura do barramento de dados - quantidade de linhas (vias) dedicadas aos dados.
	- Largura do barramento de endereços - quantidade de linhas (vias) dedicadas aos endereços.

**Capacidade limite de memória:**
Para calcular se faz:
- Quantidade de posições X Tamanho da posição = Capacidade limite de memória.
Ex:
- Largura de barramento = 16 bits -> 2¹⁶ = 65536 = 64K posições.
- Tamanho da posição = 8 bits (1 Byte).
- Capacidade limite de memória = 64k x 1 = 64kB (Kilobytes) de memória RAM.

## Interrupções
Quando a CPU pausa a execução de um programa para executar outro programa, e após o término retorna a execução do primeiro programa.

Tipos de causas:
- Temporização: Quando a aplicação explicitamente solicita uma pausa.
- Entrada e Saída (E/S): Para executar os comandos de E/S.
- Falha de software (exceção).
- Falha de hardware.

Pedido de interrupção CPU:
- CPU suspende a execução do programa atual.
- Salva o contexto (dados dos registradores da CPU).
- Define o registrador Contadr de Programa (PC) para o endereço inicial da Rotina de Tratamento de Interrupção (RTI).
- Atende (trata) a interrupção (executa RTI).
- Restaura o contexto;
- Continua o programa interrompido.

Funcionamento da interrupção:
- Programa Pincipal
	- ...
	- Instrução
	- Instrução
	- Instrução
	- Instrução **Interrupção**
	- Salvamento de Contexto
- RTI
	- Instrução
	- Instrução
	- Instrução
	- Instrução
- Programa Principal
	- Restauro de Contexto
	- Instrução
	- Instrução
	- Instrução
	- ...

# Tags
#hardware #computador #cpu
# Veja Também
- [[Sistemas de Computação]]
- [[Unidade Central de Processamento (CPU)]]