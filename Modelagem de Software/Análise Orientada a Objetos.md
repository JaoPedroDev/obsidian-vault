# Análise Orientada a Objetos
São quatro os princípios da orientação a objetos: abstração, herança, encapsulamento e polimorfismo, sendo que esse tópico traz mais destaque para os três últimos. Porém, antes mesmo de discutir os princípios, se faz necessário definir algumas questões, conforme mostrado abaixo:
- Objeto: Qualquer coisa visível ou tangível para qual a ação, pensamento ou sentimento é direcionado.
- Classe: Representação de um conjunto de objetos que possuem os atributos e comportamentos semelhantes.
- Instância: Objeto que foi criado em função de uma determinada classe.

## Princípio de Herança
O que a herança permite dentro da orientação a objetos é que uma classe Filha possa herdar Atributos e/ Comportamentos de uma classe Pai.

No exemplo da figura abaixo, temos três classes sendo representadas: **Pessoa**, **Professor** e **Aluno**. A classe **Pessoa** possui os atributos _Idade_, _Nome_ e _RG_. Ela é a superclasse das classes **Professor** e **Aluno**, que foram especializadas por conta dos atributos e métodos particulares existentes para cada tipo de objeto.

![](https://i.imgur.com/enUJMOw.png)

## Princípio do Encapsulamento
O objetivo do princípio de Encapsulamento é ocultar dados e/ou operações existentes em uma classe. A ideia de ocultar tais características e/ou comportamentos tem forte relação com segurança do objeto. Dessa maneira, o objeto só terá disponível conteúdos realmente necessários para sua interação.

## Princípio do Polimorfismo
A orientação a objetos permite que uma subclasse possa alterar o comportamento / forma como a sua superclasse executa determinada operação, mantendo o mesmo nome de operação. Essa possibilidade implica em um sistema poder ter múltiplas formas de execução.

O exemplo abaixo mostra a capacidade do polimorfismo. A superclasse Figura Geométrica é apenas uma simplificação do objeto real, indicando que toda figura geométrica tem uma quantidade de lados e que toda figura geométrica tem a operação _Desenha_. Entretanto, entende-se que a operação _Desenha_ irá modificar o seu comportamento de acordo com o tipo de figura geométrica que estiver sendo desenhada.

![](https://i.imgur.com/BQIFQGu.png)

# Tags
#desenvolvimento #software #linguagemdeprogramacao 
# Veja Também
- [[Metodologias de Desenvolvimento de Sistemas]]
- [[OOP - Abstração]]
- [[OOP - Atributos]]
- [[OOP - Operações]]
- [[OOP - Classe e Objetos]]
- [[OOP - Associação]]
- [[OOP - Diagrama de Casos de Uso]]