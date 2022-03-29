# OOP - Diagrama de Pacotes
Na [[Análise Orientada a Objetos]] é necessário a criação de inúmeras classes para representar os elementos do sistema, e essas classes podem ter diferentes objetivos, sendo assim, surgiram os pacotes, que servem para organizar subsistemas existentes dentro do sistema que está sendo modelado, permitindo a visualização da organização dos subsistemas modelados.

Com isso, o diagrama de pacotes mostra a decomposição do sistema, indicando suas dependências.

Dentro de um pacote é possível adicionar outros elementos conhecidos da UML, como classes, interfaces, componentes, nós, casos de uso, diagramas e até outros diagramas de pacotes.

A figura abaixo representa um sistema que trabalha com o conceito de três camadas, tendo pacotes distintos para a interface gŕafica, regra de negócio e acesso a dados.
![](https://i.imgur.com/7NHXr2h.png)

A ideia é que exista uma tela de cadastro de usuários, que atendo à assinatura de um Formulário. Essa tela passa informações para a classe do negócio dedicada para o usuário. Em seguida, após a aplicação das regras de negócio necessárias, a classe de acesso a dados dedicada para o usuário faz o acionamento do banco de dados de usuário.
# Tags
#orientacaoaobjetos #desenvolvimento #software 
# Veja Também
- [[Análise Orientada a Objetos]]