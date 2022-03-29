# Metodologias de Desenvolvimento de Sistemas
Desenvolver softwares utilizando conceitos de engenharia. Essa é a maneira hoje utilizada dentro das organizações para tentar evitar o que ficou conhecido como Crise do Software. Números mais atuais indicam que mais de 60% dos projetos de software falham! Desses, 20% a 25% são cancelados ou não chegam a ser usados. Fica então a pergunta – Como melhorar esses percentuais?

A Engenharia de Software surgiu com essa perspectiva. O fato é que a Engenharia de Software defende atividades fundamentais para a construção de um programa, chamado também de ciclo de vida do projeto de software. Veja abaixo cada uma das etapas fundamentais de um projeto de software.

![](https://i.imgur.com/hmitY3d.png)

## Análise Estruturada
Abordagem voltada para os aspectos funcionais e de dados do sistema.

A análise estruturada tem como artefatos produzidos os diagramas de Entidade-Relacionamento (DER) e de Fluxo de Dados (DFD). Além disso, espera-se a construção de um Dicionário de Dados. Conceitualmente, espera-se a construção do sistema de forma _top-down_ (do todo para as partes).

### Exemplo diagram de fluxo de dados
![](https://i.imgur.com/202zQSi.png)

### Exemplo de diagram de entidade-relacionamento
![](https://i.imgur.com/J5X8lZP.png)

## Análise Essencial
É a evolução da Análise Estruturada, adiciona a questão do Controle como aspecto a ser modelado além das Funções e dos Dados. É formada por dois modelos:
- Modelo Ambiental: Composto pelo Diagram de Contexto, por uma lista de eventos e pela descrição dos objetivos do sistema.
- Modelo Comportamental: Composto pelo Diagrama de Fluxo de Dados, o Diagrama Entidade Relacionamento, o Diagrama de Transição de Estados e pelo Dicionário de Dados.

### Exemplo de diagrama de contexto
![](https://i.imgur.com/8zbbqDH.png)

### Exemplo de diagrama de transição de estados
![](https://i.imgur.com/nQdl4jM.png)

## [[Análise Orientada a Objetos]]
Um sistema construído usando um método Orientado a Objetos é aquele cujos componentes são partes encapsuladas de dados e funções, que podem herdar atributos e comportamentos de outros componentes da mesma natureza, e cujos componentes comunicam-se entre si por meio de mensagens.

O método de modelagem passa a ser bottom-up. Na orientação a objetos a representação de um conjunto de objtos com características (dados / atributos) e comportamentos (funções / métodos) semelhantes é chamada de Classe.
![](https://i.imgur.com/gSllukM.png)

# Tags
#desenvolvimento #software
# Veja Também
- [[Sistemas de Computação]]
- [[Análise Orientada a Objetos]]