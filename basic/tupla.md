Tuplas Python
mytuple = ("apple", "banana", "cherry")
Tupla
Tuplas são usadas para armazenar vários itens em uma única variável.

Tuple é um dos 4 tipos de dados internos do Python usados ​​para armazenar coleções de dados, os outros 3 são List , Set e Dictionary , todos com qualidades e usos diferentes.

Uma tupla é uma coleção ordenada e imutável .

Tuplas são escritas com colchetes.

Exemplo
Crie uma Tupla:

thistuple = ("apple", "banana", "cherry")
print(thistuple)
Itens de Tupla
Os itens de tupla são ordenados, imutáveis ​​e permitem valores duplicados.

Os itens de tupla são indexados, o primeiro item possui índice [0], o segundo item possui índice [1]etc.

Encomendado
Quando dizemos que as tuplas estão ordenadas, significa que os itens têm uma ordem definida, e essa ordem não será alterada.

Imutável
As tuplas são imutáveis, o que significa que não podemos alterar, adicionar ou remover itens após a criação da tupla.

Permitir duplicatas
Como as tuplas são indexadas, elas podem ter itens com o mesmo valor:

Exemplo
Tuplas permitem valores duplicados:

thistuple = ("apple", "banana", "cherry", "apple", "cherry")
print(thistuple)
PROPAGANDA

Comprimento da Tupla
Para determinar quantos itens uma tupla possui, use a len()função:

Exemplo
Imprima o número de itens na tupla:

thistuple = ("apple", "banana", "cherry")
print(len(thistuple))
Criar Tupla Com Um Item
Para criar uma tupla com apenas um item, você deve adicionar uma vírgula após o item, caso contrário, o Python não o reconhecerá como uma tupla.

Exemplo
Uma tupla de item, lembre-se da vírgula:

thistuple = ("apple",)
print(type(thistuple))

#NOT a tuple
thistuple = ("apple")
print(type(thistuple))
Itens de Tupla - Tipos de Dados
Os itens de tupla podem ser de qualquer tipo de dados:

Exemplo
Tipos de dados String, int e boolean:

tuple1 = ("apple", "banana", "cherry")
tuple2 = (1, 5, 7, 9, 3)
tuple3 = (True, False, False)
Uma tupla pode conter diferentes tipos de dados:

Exemplo
Uma tupla com strings, inteiros e valores booleanos:

tuple1 = ("abc", 34, True, 40, "male")
tipo()
Da perspectiva do Python, as tuplas são definidas como objetos com o tipo de dados 'tupla':

<class 'tuple'>
Exemplo
Qual é o tipo de dados de uma tupla?

mytuple = ("apple", "banana", "cherry")
print(type(mytuple))
O construtor tupla()
Também é possível usar o construtor tuple() para fazer uma tupla.

Exemplo
Usando o método tuple() para fazer uma tupla:

thistuple = tuple(("apple", "banana", "cherry")) # note the double round-brackets
print(thistuple)
Coleções Python (matrizes)
Existem quatro tipos de dados de coleção na linguagem de programação Python:

Lista é uma coleção que é ordenada e mutável. Permite membros duplicados.
Tupla é uma coleção ordenada e imutável. Permite membros duplicados.
Set é uma coleção não ordenada, imutável* e não indexada. Nenhum membro duplicado.
Dicionário é uma coleção ordenada** e mutável. Nenhum membro duplicado.
*Os itens do conjunto são imutáveis, mas você pode remover e/ou adicionar itens sempre que quiser.

**A partir da versão 3.7 do Python, os dicionários são ordenados . No Python 3.6 e anteriores, os dicionários não são ordenados .

Ao escolher um tipo de coleção, é útil entender as propriedades desse tipo. Escolher o tipo certo para um determinado conjunto de dados pode significar retenção de significado e pode significar um aumento na eficiência ou segurança.

Python - Acessar itens de tupla
Acessar itens de tupla
Você pode acessar os itens da tupla consultando o número do índice, entre colchetes:

Exemplo
Imprima o segundo item na tupla:

thistuple = ("apple", "banana", "cherry")
print(thistuple[1])
Nota: O primeiro item tem índice 0.

Indexação negativa
Indexação negativa significa começar do fim.

-1refere-se ao último item, -2refere-se ao penúltimo item etc.

Exemplo
Imprima o último item da tupla:

thistuple = ("apple", "banana", "cherry")
print(thistuple[-1])
Faixa de índices
Você pode especificar um intervalo de índices especificando onde começar e onde terminar o intervalo.

Ao especificar um intervalo, o valor de retorno será uma nova tupla com os itens especificados.

Exemplo
Retorne o terceiro, quarto e quinto item:

thistuple = ("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")
print(thistuple[2:5])
Nota: A pesquisa começará no índice 2 (incluído) e terminará no índice 5 (não incluído).

Lembre-se que o primeiro item tem índice 0.

Ao deixar de fora o valor inicial, o intervalo começará no primeiro item:

Exemplo
Este exemplo retorna os itens do início para, mas NÃO inclui, "kiwi":

thistuple = ("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")
print(thistuple[:4])
Ao deixar de fora o valor final, o intervalo irá para o final da lista:

Exemplo
Este exemplo retorna os itens de "cherry" e até o final:

thistuple = ("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")
print(thistuple[2:])
PROPAGANDA

Faixa de índices negativos
Especifique índices negativos se desejar iniciar a pesquisa a partir do final da tupla:

Exemplo
Este exemplo retorna os itens do índice -4 (incluído) ao índice -1 (excluído)

thistuple = ("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")
print(thistuple[-4:-1])
Verifique se o item existe
Para determinar se um item especificado está presente em uma tupla, use a inpalavra-chave:

Exemplo
Verifique se "apple" está presente na tupla:

thistuple = ("apple", "banana", "cherry")
if "apple" in thistuple:
  print("Yes, 'apple' is in the fruits tuple")

Python - Atualizar Tuplas
As tuplas são imutáveis, o que significa que você não pode alterar, adicionar ou remover itens depois que a tupla for criada.

Mas existem algumas soluções alternativas.

Alterar valores da tupla
Depois que uma tupla é criada, você não pode alterar seus valores. Tuplas são imutáveis , ou imutáveis , como também é chamado.

Mas há uma solução alternativa. Você pode converter a tupla em uma lista, alterar a lista e convertê-la novamente em uma tupla.

Exemplo
Converta a tupla em uma lista para poder alterá-la:

x = ("apple", "banana", "cherry")
y = list(x)
y[1] = "kiwi"
x = tuple(y)

print(x)
Adicionar itens
Como as tuplas são imutáveis, elas não possuem um append()método embutido, mas existem outras maneiras de adicionar itens a uma tupla.

1. Converter em uma lista : Assim como a solução alternativa para alterar uma tupla, você pode convertê-la em uma lista, adicionar seu(s) item(ns) e convertê-la novamente em uma tupla.

Exemplo
Converta a tupla em uma lista, adicione "laranja" e converta novamente em uma tupla:

thistuple = ("apple", "banana", "cherry")
y = list(thistuple)
y.append("orange")
thistuple = tuple(y)
2. Adicionar tupla a uma tupla . Você tem permissão para adicionar tuplas a tuplas, portanto, se você quiser adicionar um item (ou muitos), crie uma nova tupla com o(s) item(ns) e adicione-a à tupla existente:

Exemplo
Crie uma nova tupla com o valor "laranja" e adicione essa tupla:

thistuple = ("apple", "banana", "cherry")
y = ("orange",)
thistuple += y

print(thistuple)
Nota: Ao criar uma tupla com apenas um item, lembre-se de incluir uma vírgula após o item, caso contrário ele não será identificado como uma tupla.

PROPAGANDA

Remover itens
Nota: Você não pode remover itens em uma tupla.

As tuplas não podem ser alteradas , portanto, você não pode remover itens dela, mas pode usar a mesma solução alternativa que usamos para alterar e adicionar itens de tupla:

Exemplo
Converta a tupla em uma lista, remova "apple" e converta-a novamente em uma tupla:

thistuple = ("apple", "banana", "cherry")
y = list(thistuple)
y.remove("apple")
thistuple = tuple(y)
Ou você pode excluir a tupla completamente:

Exemplo
A delpalavra-chave pode excluir a tupla completamente:

thistuple = ("apple", "banana", "cherry")
del thistuple
print(thistuple) #this will raise an error because the tuple no longer exists

Python - Descompacte Tuplas
Descompactando uma Tupla
Quando criamos uma tupla, normalmente atribuímos valores a ela. Isso é chamado de "empacotar" uma tupla:

Exemplo
Empacotando uma tupla:

fruits = ("apple", "banana", "cherry")
Mas, em Python, também podemos extrair os valores de volta para as variáveis. Isso é chamado de "descompactar":

Exemplo
Descompactando uma tupla:

fruits = ("apple", "banana", "cherry")

(green, yellow, red) = fruits

print(green)
print(yellow)
print(red)
Nota: O número de variáveis ​​deve corresponder ao número de valores na tupla, caso contrário, você deve usar um asterisco para coletar os valores restantes como uma lista.

PROPAGANDA

Usando asterisco*
Se o número de variáveis ​​for menor que o número de valores, você pode adicionar um *ao nome da variável e os valores serão atribuídos à variável como uma lista:

Exemplo
Atribua o restante dos valores como uma lista chamada "red":

fruits = ("apple", "banana", "cherry", "strawberry", "raspberry")

(green, yellow, *red) = fruits

print(green)
print(yellow)
print(red)
Se o asterisco for adicionado a outro nome de variável que não o último, o Python atribuirá valores à variável até que o número de valores restantes corresponda ao número de variáveis ​​restantes.

Exemplo
Adicione uma lista de valores a variável "tropic":

fruits = ("apple", "mango", "papaya", "pineapple", "cherry")

(green, *tropic, red) = fruits

print(green)
print(tropic)
print(red)

Python - Tuplas de Loop
Percorrer uma Tupla
Você pode percorrer os itens da tupla usando um forloop.

Exemplo
Iterar pelos itens e imprimir os valores:

thistuple = ("apple", "banana", "cherry")
for x in thistuple:
  print(x)
Saiba mais sobre forloops em nosso capítulo Python For Loops .

Percorrer os números de índice
Você também pode percorrer os itens da tupla consultando seu número de índice.

Use as funções range()e len()para criar um iterável adequado.

Exemplo
Imprima todos os itens consultando seu número de índice:

thistuple = ("apple", "banana", "cherry")
for i in range(len(thistuple)):
  print(thistuple[i])
PROPAGANDA

Usando um loop while
Você pode percorrer os itens da lista usando um whileloop.

Use a len()função para determinar o comprimento da tupla, então comece em 0 e faça um loop pelos itens da tupla consultando seus índices.

Lembre-se de aumentar o índice em 1 após cada iteração.

Exemplo
Imprima todos os itens, usando um whileloop para percorrer todos os números de índice:

thistuple = ("apple", "banana", "cherry")
i = 0
while i < len(thistuple):
  print(thistuple[i])
  i = i + 1
Saiba mais sobre whileloops em nosso capítulo Python While Loops .

Python - Junte Tuplas
Junte-se a duas tuplas
Para juntar duas ou mais tuplas você pode usar o + operador:

Exemplo
Junte duas tuplas:

tuple1 = ("a", "b" , "c")
tuple2 = (1, 2, 3)

tuple3 = tuple1 + tuple2
print(tuple3)
Multiplicar Tuplas
Se você quiser multiplicar o conteúdo de uma tupla um determinado número de vezes, você pode usar o * operador:

Exemplo
Multiplique a tupla de frutas por 2:

fruits = ("apple", "banana", "cherry")
mytuple = fruits * 2

print(mytuple)

Python - Métodos de Tupla
Métodos de Tupla
Python tem dois métodos integrados que você pode usar em tuplas.

Method	Description
count()	Returns the number of times a specified value occurs in a tuple
index()	Searches the tuple for a specified value and returns the position of where it was found