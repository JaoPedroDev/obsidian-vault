# OOP - Associação
Existem diferentes tipos de associações entre classes. Cada uma com seu respectivo propósito.

## Associação Unária (Auto relacionamento)
Utilizada quando um objeto precisa possuir como propriedade um ou mais objetos de mesma característica (classe). O exemplo abaixo mostra o conceito de um gerente, responsável por um ou mais funcionários. A sua ligação é feita através de uma seta que liga a classe a ela mesma.
![](https://i.imgur.com/XA7FMtm.png)

## Associação Binária
Relacionamento simples entre duas classes. O exemplo indica a relação existente entre os departamentos de uma organização e os seus funcionários. A sua ligação é feita através de uma seta que liga as classes associadas.
![](https://i.imgur.com/Sp32Y5K.png)

# Generalização
Onde é aplicada a herança. A herança múltipla é possível, porém incomum devido a limitações de algumas linguagens de programação. Essa associação descreve uma relação "É UM".
![](https://i.imgur.com/02InLC0.png)

# Dependência
Indica o grau de dependência entre classes. Esses relacionamentos podem expressar também ordem de precedência, onde um elemento deve preceder a outro.
![](https://i.imgur.com/PENX4co.png)

# Agregação
A ideia de agregação é mostrar o relacionamento entre as classes conforme elas vão se agregando uma nas outras. É possível agregar inúmeras classes a uma única classe e uma classe agregadora pode ainda ser agregada a outra classe.
O grande detalhe do relacionamento de agregação é que, apesar da classe agregadora ter uma visão única do todo, não será ela que controlará as partes, ou seja, as classes que estão sendo agregadas. Esse controle diz respeito à instanciação ou destruição das classes, por exemplo.
O exemplo abaixo mostra a evolução da representação do relacionamento entre departamento e funcionário. A representação da agregação é feita por uma linha que possui um losango sem preenchimento na classe responsável pela agregação.
![](https://i.imgur.com/HVTnmp8.png)

## Composição
É uma especialização da agregação, que indica que a classe que está compondo a entidade que se deseja representar será responsável pelo controle da classe que está sendo composta. A representação da composição é feita por uma linha que possui um losango com preenchimento na classe responsável pela composição.
![](https://i.imgur.com/RmNdepE.png)

# Tags
#orientacaoaobjetos #software 
# Veja Também
- [[Análise Orientada a Objetos]]
- [[OOP - Classe e Objetos]]