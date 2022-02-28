Tipos de dados Python
Tipos de dados integrados
Na programação, o tipo de dados é um conceito importante.

Variáveis ​​podem armazenar dados de diferentes tipos, e diferentes tipos podem fazer coisas diferentes.

O Python tem os seguintes tipos de dados integrados por padrão, nestas categorias:

Tipo de texto:	str
Tipos Numéricos:	int, float, complex
Tipos de sequência:	list, tuple, range
Tipo de mapeamento:	dict
Tipos de conjunto:	set,frozenset
Tipo booleano:	bool
Tipos binários:	bytes, bytearray, memoryview
Obtendo o tipo de dados
Você pode obter o tipo de dados de qualquer objeto usando a type()função:

Exemplo
Imprima o tipo de dados da variável x:

x = 5
print(type(x))
Configurando o tipo de dados
Em Python, o tipo de dados é definido quando você atribui um valor a uma variável:

Example	Data Type	Try it
x = "Hello World"	str	
x = 20	int	
x = 20.5	float	
x = 1j	complex	
x = ["apple", "banana", "cherry"]	list	
x = ("apple", "banana", "cherry")	tuple	
x = range(6)	range	
x = {"name" : "John", "age" : 36}	dict	
x = {"apple", "banana", "cherry"}	set	
x = frozenset({"apple", "banana", "cherry"})	frozenset	
x = True	bool	
x = b"Hello"	bytes	
x = bytearray(5)	bytearray	
x = memoryview(bytes(5))	memoryview

Configurando o tipo de dados específico
Se você deseja especificar o tipo de dados, pode usar as seguintes funções de construtor:

Example	Data Type	Try it
x = str("Hello World")	str	
x = int(20)	int	
x = float(20.5)	float	
x = complex(1j)	complex	
x = list(("apple", "banana", "cherry"))	list	
x = tuple(("apple", "banana", "cherry"))	tuple	
x = range(6)	range	
x = dict(name="John", age=36)	dict	
x = set(("apple", "banana", "cherry"))	set	
x = frozenset(("apple", "banana", "cherry"))	frozenset	
x = bool(5)	bool	
x = bytes(5)	bytes	
x = bytearray(5)	bytearray	
x = memoryview(bytes(5))	memoryview
