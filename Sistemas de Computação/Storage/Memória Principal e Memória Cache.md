# Memória Principal e Memória Cache
Há dois tipos de memória RAM:
- Dinâmica - DRAM: os dados são gravados como cargas elétricas em capacitores. A quantidade de cargas determina se o valor armazenado corresponde ao bit 0, ou ao bit 1, sendo assim, uma memória analógica. Usada como **Memória Principal**
- Estática - SRAM: o bit é armazenado através de um esquema de chaves eletrônicas feitas com transistores, que mantém o dado enquanto o circuito estiver energizado, sendo uma memória totalmente digital. Usada como **Memória Cache**

## Memória Principal
Ela é responsavel por armazenar os programas durante sua execução. Por isso é importante ter um bom desempenho, sendo empregadas algumas técnicas para melhorar sua velocidade.

- SDRAM - RAM Dinâmica Síncrona: Emprega sinal de clock para sincronizar as operações e melhorar o desempenho.
- DDR - Double Data Rate (DDR-SDRAM): Permite que os dados sejam transferidos quando o clock vai de 0 para 1 (transição de subida) e de 1 para 0 (transição de descida), resultando em uma taxa de dados duplicada.
- Multi Channel: Melhora o desempenho da memória acessando mais de uma posição de memória ao mesmo tempo, cada uma através de uma canal de memória.

## Memória Cache
É uma memória RAM estática (SRAM) de altíssimo desempenho que fica localizada dentro da [[Unidade Central de Processamento (CPU)]]. E funciona da seguinte forma:
- A CPU requisita à memória o conteúdo de uma determinada posição.
- O controle do cache verifica se aqueles dados estão disponíveis no cache.
- Se estiberem, fornce o dado à CPU(rápido).
- Se não, lê o bloco de dados solicitado na memória principal e copia para o cache, para só então fornecer os dados à CPU.

Para saber a informação a ser guardade na memória cache, são empregados dois Princípios de Localidade:
- Principio de Localidade Temporal: Uma vez acessada uma determinada posição de memória, ela tende a ser acessada outra vez no futuro próximo.
- Principio de Localidade Espacial: Uma vez acessada uma determinada posição de memória, as posições subsequentes tendem a ser acessadas no futuro próximo.

# Tags
#hardware #computador #armazenamento 
# Veja Também
- [[Sistema de Armazenamento (Memórias)]]
- [[Sistemas de Computação]]
- [[Unidade Central de Processamento (CPU)]]