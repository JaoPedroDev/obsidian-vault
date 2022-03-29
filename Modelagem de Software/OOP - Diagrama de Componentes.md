# OOP - Diagrama de Componentes
Diagrama que possui como foco o desenvolvimento de componentes que possam operar sozinhos, assim podendo ser reutilizados em outros projetos.

Componente é definido como a parte lógica e substituível de um sistema, que possa atender e prover a realização de um conjunto de interfaces.

Existem diferentes abordagens que apoiam o reuso, elas se resumem à componentização.
- Bibliotecas
- _Frameworks_
- Softwares de prateleira
- Desenvolvimento orientado a objetos
- Desenvolvimento orientado a serviços
- Desenvolvimento orientado a aspectos
- _Design Patterns_

Sendo assim, o diagrama de componentes é utilizado para modelar os componentes existentes no sistema, bem como o relacionamento entre eles através de interfaces.

É importante mencionar que as interfaces são coleções de operações que especificam um serviço que é provido ou é requerido por uma classe ou componente.

A figura abaixo apresenta os elementos de um diagrama de componentes. Existem duas representações possíveis, conforme visto abaixo.
![](https://i.imgur.com/GUM7ix0.png)

Em seguida, pode ser visto um exemplo de representação de um diagrama de componentes para um sistema que permite a utilização tanto de uma conexão Oracle como MS SQL Server. Alguns sistemas de gerenciamento de conteúdo fazem uso dessa modelagem para permitir diferentes tipos de banco de dados para o seu sistema.
![](https://i.imgur.com/OXzZzUp.png)

Abaixo também existe a representação de um componente Validador que requer uma interface de Validação para realizar sua função. A ideia é que qualquer classe / objeto que implementar a interface IValidação poderá ser utilizado pelo componente Validador para executar um regra. No caso do exemplo, existe um componente dedicado para a validação do CPF.
![](https://i.imgur.com/T35ZfQU.png)

# Tags
#orientacaoaobjetos #desenvolvimento #software 
# Veja Também
- [[Análise Orientada a Objetos]]