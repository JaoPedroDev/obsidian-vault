# OOP - Diagrama de Classes
A UML é a linguagem unificada para modelagem de sistemas, concebida para especificar, visualizar e documentar softwares, incluindo sua estrutura, comportamento e interação. Sendo assim, um dos aspectos importantes abordado por ela é a definição da estrutura do sistema.

O diagrama de classes é a solução mais utilizada para representar essa organização estrutural. Isso se deve à sua capacidade de representar os relacionamentos existentes dentro do sistema.

## Uso de Interfaces
O diagrama de classes pode também representar as interfaces do sistema.

As interfaces podem ser entendidas como abstrações de contratos que serão respeitados pelas classes concretas que a implementarão. Elas irão auxiliar na modelagem de um sistema com baixo acoplamento.

Dentro do diagrama de classes é possível definir tanto as interfaces que serão providas por uma classes como aquelas que serão requeridas. A UML trata essa questão com o que chamamos de esteriótipos de componentes visuais, ou seja, podemos utilizar o mesmo componente visual utilizado para representar uma classe na representação de uma interface, apenas sinalizando que essa classe na verdade não é uma classe, mas sim um estereótipo da classe, representando uma interface. A figura abaixo mostra a implementação de uma interface provida chamada "IExemplo". Notem que é possível fazer a representação através do estereótipo ou através do componente visual específico que define uma interface.
![](https://i.imgur.com/fqZgjiZ.png)

A segunda imagem mostra o uso de uma interface requerida pela classe Teste, também mostrando o componente visual utilizado pra indicar interfaces requeridas.
![](https://i.imgur.com/KNUOGVQ.png)

## Exemplo
Diagrama de Casos de Uso do Sistema de Gerenciamento de Reclamações
![](https://i.imgur.com/1mdiJB1.png)

# Tags
#desenvolvimento #software #orientacaoaobjetos 
# Veja Também
- [[OOP - Diagrama de Casos de Uso]]
- [[Análise Orientada a Objetos]]