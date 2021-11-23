# Sistemas de Entrada e Saída (E/S)
São os sistemas que controlam a entrada e saída de informações (Audio, Video, Imagem, Arquivos, etc). Eles são 

## Módulo de E/S
Os módulos de E/S são conectados a [[Unidade Central de Processamento (CPU)]] através do [[Sistema de Interconexão (Barramentos)]], e são as ligações do sistema computacional com o mundo externo. Razões para não ligar o periférico diretamente ao barramento:
- Grande variedade de periféricos, com diferentes lógicas de operação.
- Dispositivos externos possuem uma taxa de transferência de dados muito menor que aquela estabelecida entre a CPU e a memória.
- O formato dos dados e o tamanho das palavras usados pelos periféricos podem ser diferentes dos utilizados pelo computador.

As funções de um módulo de E/S:
- Controle e temporização
- Comunicação com a CPU
- Comunicação com os periféricos
- Armazenamento temporário de dados
- Detecção de erros

O intuito do módulo de E/S é dar ao processador uma visão simplificada da grande variedade de periféricos.

Ao exexutar uma operação de E/S, a CPU envia um comando para o módulo de E/S apropriado, solicitando uma operação especifica.
Os tipos de comandos de E/S são:
- Controle: Ativa um periférico e indica uma ação
- Teste: Verifica as condições de estado do periférico
- Leitura: Solicita a leitura de itens de dados do periférico
- Gravação: CPU ordena ao módulo de E/S que pegue o dado do barramento de dados e o armazene no periférico

## Periféricos
Existem diversos tipos de dispositivos externos. Eles podem ser divididos em:
- Voltados para comunicação com o usuário: Teclado, vídeo, impressora, etc
- Voltados para comunicação com a máquina: Discos magnéticos, sensores, etc.
- Voltados para a comunicação com dispositivos remotos: Modem, placa de rede, etc.

Na comunicação do periférico com a CPU, as seguintes etapas estão envolvidas:
- A CPU interroga o módulo de E/S sobre o estado do periférico
- O módulo de E/s informa o estado do periférico à CPU
- Se o dispositivo estiver pronto, o processador solicita a transferência dos dados enviando um comando para o módulo de E/S
- Uma palavra de dados é obtida do periférico pelo módulo de E/S
- O módulo de E/S transfere os dados para a CPU

## Técnicas de Operações de E/s
Existem três técnicas diferentes que podem ser utilizadas durante a realização de operações de E/S, são elas:

### E/S Programada
A CPU, além de executar o programas, possui controle total sobre as operações de E/S. Isso inclui:
- A detecção do estado do periférico
- O envio de comandos para o módulo de E/S
- Transferência de dados

É uma técnica lentas, pois o processador necessita pausar a execução do programa para esperar pela ação da E/S, que é muito mais lento que o processador.

### E/S Dirigida por Interrupção
A CPU envia um sinal para o módulo de E/S com a operação solicitada e continua a execução dor programas, quando a operação estiver pronta no módulo de E/S, ele envia um sinal para a CPU, que realiza a tranferência dos dados. Dessa forma não há lentidão.

### DMA - Acesso Direto à memória
Direct Memory Access(DMA) é um sistema utilizado quando há a necessidade de uma grande transferência de dados, geralmente entre a memória secundária e a memória principal. Com essa técnica a CPU apenas indica o começo e o fim da tranferência, ao invés de lidar com cada palavra de dados.

As informações trocadas entre o módulo de E/S com DMA e a CPU quando esta deseja ler ou escrever um conjunto de dados em um periférico podem ser descritas como segue:
- Por meio do barramento de controle a CPU indica o tipo de operação ao DMA
- É fornecido o endereço do módulo de E/S correspondente
- É fornecido o endereço de memória par ao módulo DMA armazenar ou ler os dados
- É fornecida a quantidade de palavras que serão lidas ou escritas

# Tags
#hardware #computador #cpu 
# Veja Também
- [[Sistemas de Computação]]
- [[Sistema de Interconexão (Barramentos)]]