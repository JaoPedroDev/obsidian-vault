# OOP - Diagrama de Estrutura Composta
Apresenta a estrutura interna de uma classe ou colaboração. A diferença desse diagrama para o diagrama de componentes é muito pequena, por isso muitos analistas quando realizam a modelagem acabam não se utilizando desse diagrama.

É formado pelos elementos abaixo:
- **Classe estruturada**: Representa a classe que se deseja apresentar a estrutura interna;
- **Parte**: Indica um elemento necessário para a classe estruturada que está sendo modelada;
- **Porta**: Ponto de conexão entre a classe que está sendo detalhada e o mundo externo;
- **Interface requerida**: Indica uma interface necessária para compor a classe que está sendo modelada;
- **Interface provida**: Indica uma interface que está sendo fornecida para a classe que está sendo detalhada.

Abaixo exemplifica a estrutura da classe Interruptor, composta pelas partes de uma chave liga / desliga e de um LED para sinalização. Por tal razão, essa classe requer as interfaces IChaveLigaDesliga e ILed. Essas interfaces estão sendo providas pelas classes ChaveOnOff e Led.
![](https://i.imgur.com/2KGWmQz.png)


# Tags
#orientacaoaobjetos #software #desenvolvimento 
# Veja Também
- [[Análise Orientada a Objetos]]