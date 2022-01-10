# Python
Linguagem de programação de alto nível, interpretada de script, imperativa, orientada a objetos, funcional, de tipagem dinâmica e forte.

Digitar "python" no terminal abre o interpretador interativo. Python lê o que for escrito e apresenta o resultado.

## Tipos de Dados
Python suporta todos os tipos de dados básicos, e também possui dados compostos:
### Integers:
```python
	1 + 2
	#return 3
```

### Floating point:
```python
	1.5 + 2.5
	#return 4.0
```

### Strings:
```python
	#duas
	"hello world"
	
	'hello world'
	
	#Strings podem ser multiplicadas
	print("hello" * 5)
	#return hellohellohellohellohello
```

Strings podem ser comparadas
Elas obedecem a ordem alfabética de cada letra.
```python
	"a" < "b"
	#return True
	"b" > "c"
	#return False
```

Strings multilinhas
```python
	""" Essa é uma
	menssagem em
	varias linhas
	"""
```

Escape codes
"\n" indica nova linha
"\t" indica um tab

### [[Python - Listas]]:
```python
	x = ["a", "b", "c"]
	
	x[1]
	#return 'b'
```
Listas podem ser heterogeneas
```python
	x = ["ola", 1, 2, "word", ["another", "list"]]
```

### Tuples:
Usado para armazenar registro de largura fixos. São como listas, mas não podem ser alterados.
```python
	point = (1, 3)
	# or
	point = 1, 3
	point
	#return (1, 3)
	
	#multiplos valores
	yellow = (255, 255, 0)
	r, g, b = yellow
	print(r, g, b)
	#return 255 255 0
```

### Dicionário:
```python
	person = {"name": "Alice", "email": "alice@exemple.com"}
	person['name']
	#return 'Alice'
```

### Set:
Coleção de elementos não ordenados
```python
	x = {1, 2, 3, 2, 1}
	x
	#return x
	{1, 2, 3}
```

### Boolean:
Representa dois valores, Verdadeiro ou Falso

### None:
Presenta "nada" ou vazio
```python
	x = None
	print(x)
	#return None
```

## Variaveis
Em Python variaveis não possuem tipo, são apenas placeholders que podem guardar qualquer tipo de dados.
```python
	x = 5
	x
	#return 5
```

## Funções
len():
Retorna a quantidade de elementos de uma string, lista ou outras coleções
```python
	len("hello")
	#return 5
	
	len(['a', 'b', 'c'])
	#return 3
```

Python não aceita operações de tipo de dados diferentes, para isso possui funções de conversão de tipo de dados.
```python
	int("5")
	#return 5
	
	str(5)
	#return '5'
	
	str(5) + "2"
	#return '52'
```

Contando o número de digitos em um número:
```python
	len(str(12345))
	#return 5
	
	len(str(2 ** 100))  #quantidade de digitos de 2 elevado a 100
	#return 31
```

### Escrevendo as próprias funções:
```Python
	def square(x):
		return x * x
		
	square(5)
	#return 25
```
**Nessecita de identação**, python usa a identação para dividir os blocos de código.

Funções podem ser passadas como argumentos.
```Python
	f = square
	f(4)
	#return 16
```

Variaveis globais só podem ser lidas dentro das funções
```Python
	x = 0
	y = 0
	def incr(x):
    	y = x + 1
    	return y
	incr(5)
	print x, y
	#return 0, 0
```
Para altera-las é necessario declarar explicitamente que são globais
```Python
	numcalls = 0
	def square(x):
		global numcalls
		numcalls = numcalls + 1
		return x * x
	#return 
```

### Lambda operator
```Python
	cube = lambda x: x ** 3
	fxy(cube, 2, 3)
	#return 35
	
	fxy(lambda x: x ** 3, 2, 3)
	#return 35
```

Lambda não precisa de um "return", é uma expressão única.
Usado frequentemente quando é necessário funções pequenas a serem passadas como argumentos.
# Tags
#linguagemdeprogramacao #computador
# Veja Também
- 