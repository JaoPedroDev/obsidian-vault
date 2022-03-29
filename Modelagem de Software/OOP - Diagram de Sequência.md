# OOP - Diagrama de Sequência
É uma das ferramentas mais conhecidas para se representar a interação de um sistema orientado a objetos. Ele enfatiza a ordem de chamada das operações em uma determinada situação do sistema em função do tempo.

Essa característica faz com que o diagrama tenha um conceito de linha do tempo e de execução das operações.
![](https://i.imgur.com/6GrtojB.png)

Estereótipos para representar as classes na linha do tempo:
- Ator: Usuário ou outro sistema interagindo com o sistema;
- Interface: Faz a troca de mensagens com o ator.
- Controle: Possui a lógica de negócio do sistema para a sequência modelada;
- Entidade: Armazena o conteúdo das entidades que estão sendo tratadas por aquele sistema.

Esse diagrama ainda pode definir lógicas de execução através de operadores lógicos. Os mais comuns são:
- Condição opcional (opt): Só irá acontecer o bloco lógico se a condição pré-definida for válida;
- Condição alternativa (alt): Alternativas que podem ser executadas, de acordo com pré-condições de entrada para cada uma das alternativas;
- Execução em paralelo (par): Permite representar ações acontecendo de forma concorrente;
- Execução em loop (loop): Indica que haverá um loop de execução respeitado por um alógica de atendimento do loop.
![](https://i.imgur.com/Ubg4Nfe.png)

## Exemplo de um Diagrama de Sequência
Sistema de Reclamações, considerando que o técnico está consultando a lista de reclamações para selecionar uma reclamação para começar a atuar.
![](https://i.imgur.com/UkxsxPb.png)

# Tags
#orientacaoaobjetos #software #desenvolvimento 
# Veja Também
- [[Análise Orientada a Objetos]]