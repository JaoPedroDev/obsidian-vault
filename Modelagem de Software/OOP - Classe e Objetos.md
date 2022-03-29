# OOP - Classe e Objetos
A representação de um conjunto de objetos com características e comportamentos semelhantes é chamada de Classe. Sendo assim, a classe nada mais é que uma descrição do que o objeto possui e como o objeto atua.

Os objetos são caracterizados por possuírem Identidade, Estado e Comportamento. A comunicação entre os objetos é feita através de mensagens que acionam os comportamentos definidos.

Na etapa de Análise de um sistema, a grande preocupação existente se dá pela descoberta de suas classes. A relação entre as classes vai permitir a construção de um diagrama estrutural do sistema, chamado de Diagrama de Classes.

Representação de uma classe utilizando diagramação:
![](https://i.imgur.com/oZc3D0O.png)

A classe gerada pelo diagrama é facilmente transformada em código:
```c++
	class Produto
	{
		public int CodigoBarras { get;set }
		public string Descricao { get;set }
		public float Preco { get;set }
		public void Imprimir()
		{
			# TODO - Escrever o método de impressão
		}
		
		public int ObtemQuantidadeEstoque()
		{
			# TODO - Escrever o método para 
			# obter q quantidade em estoque
			return 0;
		}

		public float CalcularSubTotal(int quantidade)
		{
			return quantidade * Preco;
		}
	}
```

Assim sendo, a Análise Orientada a Objetos simplifica a visão de como o sistema computacional será estruturado, para posteriormente ele ser codificado conforme a análise e organização definida pelo analista de sistemas.
Essa representação, quando o programa em execução, vai ser utilizada no momento em que se desejar instanciar um objeto da classe Produto. Para cada objeto desejado, uma instância será criada, permitindo que existam diferentes informações no objeto Produto instanciados, como mostrado na figura abaixo.
![](https://i.imgur.com/Gb4UniP.png)

# Tags
#desenvolvimento #orientacaoaobjetos #software 
# Veja Também
- [[Análise Orientada a Objetos]]
- [[OOP - Abstração]]