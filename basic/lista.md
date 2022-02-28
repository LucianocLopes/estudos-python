Listas Python
mylist = ["apple", "banana", "cherry"]
Lista
As listas são usadas para armazenar vários itens em uma única variável.

As listas são um dos 4 tipos de dados internos do Python usados ​​para armazenar coleções de dados, os outros 3 são Tuple , Set e Dictionary , todos com qualidades e usos diferentes.

As listas são criadas usando colchetes:

Exemplo
Crie uma lista:

thislist = ["apple", "banana", "cherry"]
print(thislist)
lista de itens
Os itens da lista são ordenados, alteráveis ​​e permitem valores duplicados.

Os itens da lista são indexados, o primeiro item possui índice [0], o segundo item possui índice [1]etc.

Encomendado
Quando dizemos que as listas estão ordenadas, significa que os itens têm uma ordem definida, e essa ordem não será alterada.

Se você adicionar novos itens a uma lista, os novos itens serão colocados no final da lista.

Nota: Existem alguns métodos de lista que irão alterar a ordem, mas em geral: a ordem dos itens não será alterada.

Mutável
A lista é mutável, o que significa que podemos alterar, adicionar e remover itens em uma lista após ela ter sido criada.

Permitir duplicatas
Como as listas são indexadas, as listas podem ter itens com o mesmo valor:

Exemplo
As listas permitem valores duplicados:

thislist = ["apple", "banana", "cherry", "apple", "cherry"]
print(thislist)
PROPAGANDA

Comprimento da lista
Para determinar quantos itens uma lista possui, use a len()função:

Exemplo
Imprima o número de itens na lista:

thislist = ["apple", "banana", "cherry"]
print(len(thislist))
Listar itens - Tipos de dados
Os itens da lista podem ser de qualquer tipo de dados:

Exemplo
Tipos de dados String, int e boolean:

list1 = ["apple", "banana", "cherry"]
list2 = [1, 5, 7, 9, 3]
list3 = [True, False, False]
Uma lista pode conter diferentes tipos de dados:

Exemplo
Uma lista com strings, números inteiros e valores booleanos:

list1 = ["abc", 34, True, 40, "male"]
tipo()
Da perspectiva do Python, as listas são definidas como objetos com o tipo de dados 'list':

<class 'list'>
Exemplo
Qual é o tipo de dados de uma lista?

mylist = ["apple", "banana", "cherry"]
print(type(mylist))
O construtor list()
Também é possível usar o construtor list() ao criar uma nova lista.

Exemplo
Usando o list()construtor para fazer uma lista:

thislist = list(("apple", "banana", "cherry")) # note the double round-brackets
print(thislist)
Coleções Python (matrizes)
Existem quatro tipos de dados de coleção na linguagem de programação Python:

Lista é uma coleção que é ordenada e mutável. Permite membros duplicados.
Tupla é uma coleção ordenada e imutável. Permite membros duplicados.
Set é uma coleção não ordenada, imutável* e não indexada. Nenhum membro duplicado.
Dicionário é uma coleção ordenada** e mutável. Nenhum membro duplicado.
*Os itens do conjunto são imutáveis, mas você pode remover e/ou adicionar itens sempre que quiser.

**A partir da versão 3.7 do Python, os dicionários são ordenados . No Python 3.6 e anteriores, os dicionários não são ordenados .

Ao escolher um tipo de coleção, é útil entender as propriedades desse tipo. Escolher o tipo certo para um determinado conjunto de dados pode significar retenção de significado e pode significar um aumento na eficiência ou segurança.

Python - Itens da Lista de Acesso
Acessar itens
Os itens da lista são indexados e você pode acessá-los consultando o número do índice:

Exemplo
Imprima o segundo item da lista:

thislist = ["apple", "banana", "cherry"]
print(thislist[1])
Nota: O primeiro item tem índice 0.

Indexação negativa
Indexação negativa significa começar do fim

-1refere-se ao último item, -2refere-se ao penúltimo item etc.

Exemplo
Imprima o último item da lista:

thislist = ["apple", "banana", "cherry"]
print(thislist[-1])
Faixa de índices
Você pode especificar um intervalo de índices especificando onde começar e onde terminar o intervalo.

Ao especificar um intervalo, o valor de retorno será uma nova lista com os itens especificados.

Exemplo
Retorne o terceiro, quarto e quinto item:

thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[2:5])
Nota: A pesquisa começará no índice 2 (incluído) e terminará no índice 5 (não incluído).

Lembre-se que o primeiro item tem índice 0.

Ao deixar de fora o valor inicial, o intervalo começará no primeiro item:

Exemplo
Este exemplo retorna os itens do início, mas NÃO incluindo, "kiwi":

thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[:4])
Ao deixar de fora o valor final, o intervalo irá para o final da lista:

Exemplo
Este exemplo retorna os itens de "cherry" até o final:

thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[2:])
PROPAGANDA

Faixa de índices negativos
Especifique índices negativos se desejar iniciar a pesquisa a partir do final da lista:

Exemplo
Este exemplo retorna os itens de "laranja" (-4) para, mas NÃO incluindo "manga" (-1):

thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[-4:-1])
Verifique se o item existe
Para determinar se um item especificado está presente em uma lista, use a inpalavra-chave:

Exemplo
Verifique se "apple" está presente na lista:

thislist = ["apple", "banana", "cherry"]
if "apple" in thislist:
  print("Yes, 'apple' is in the fruits list")

Python - Change List Items
Change Item Value
To change the value of a specific item, refer to the index number:

Example
Change the second item:

thislist = ["apple", "banana", "cherry"]
thislist[1] = "blackcurrant"
print(thislist)
Change a Range of Item Values
To change the value of items within a specific range, define a list with the new values, and refer to the range of index numbers where you want to insert the new values:

Example
Change the values "banana" and "cherry" with the values "blackcurrant" and "watermelon":

thislist = ["apple", "banana", "cherry", "orange", "kiwi", "mango"]
thislist[1:3] = ["blackcurrant", "watermelon"]
print(thislist)
If you insert more items than you replace, the new items will be inserted where you specified, and the remaining items will move accordingly:

Example
Change the second value by replacing it with two new values:

thislist = ["apple", "banana", "cherry"]
thislist[1:2] = ["blackcurrant", "watermelon"]
print(thislist)
Note: The length of the list will change when the number of items inserted does not match the number of items replaced.

If you insert less items than you replace, the new items will be inserted where you specified, and the remaining items will move accordingly:

Example
Change the second and third value by replacing it with one value:

thislist = ["apple", "banana", "cherry"]
thislist[1:3] = ["watermelon"]
print(thislist)
ADVERTISEMENT

Insert Items
To insert a new list item, without replacing any of the existing values, we can use the insert() method.

The insert() method inserts an item at the specified index:

Example
Insert "watermelon" as the third item:

thislist = ["apple", "banana", "cherry"]
thislist.insert(2, "watermelon")
print(thislist)
Note: As a result of the example above, the list will now contain 4 items.

Python - Adicionar itens de lista
Anexar itens
Para adicionar um item ao final da lista, use o método append() :

Exemplo
Usando o append()método para anexar um item:

thislist = ["apple", "banana", "cherry"]
thislist.append("orange")
print(thislist)
Inserir itens
Para inserir um item de lista em um índice especificado, use o insert()método.

O insert()método insere um item no índice especificado:

Exemplo
Insira um item como a segunda posição:

thislist = ["apple", "banana", "cherry"]
thislist.insert(1, "orange")
print(thislist)
Nota: Como resultado dos exemplos acima, as listas agora conterão 4 itens.

PROPAGANDA

Estender lista
Para anexar elementos de outra lista à lista atual, use o extend()método.

Exemplo
Adicione os elementos de tropicala thislist:

thislist = ["apple", "banana", "cherry"]
tropical = ["mango", "pineapple", "papaya"]
thislist.extend(tropical)
print(thislist)
Os elementos serão adicionados ao final da lista.

Adicionar qualquer iterável
O extend()método não precisa anexar listas , você pode adicionar qualquer objeto iterável (tuplas, conjuntos, dicionários etc.).

Exemplo
Adicionar elementos de uma tupla a uma lista:

thislist = ["apple", "banana", "cherry"]
thistuple = ("kiwi", "orange")
thislist.extend(thistuple)
print(thislist)

Python - Remove List Items
Remove Specified Item
The remove() method removes the specified item.

Example
Remove "banana":

thislist = ["apple", "banana", "cherry"]
thislist.remove("banana")
print(thislist)
Remove Specified Index
The pop() method removes the specified index.

Example
Remove the second item:

thislist = ["apple", "banana", "cherry"]
thislist.pop(1)
print(thislist)
If you do not specify the index, the pop() method removes the last item.

Example
Remove the last item:

thislist = ["apple", "banana", "cherry"]
thislist.pop()
print(thislist)
The del keyword also removes the specified index:

Example
Remove the first item:

thislist = ["apple", "banana", "cherry"]
del thislist[0]
print(thislist)
The del keyword can also delete the list completely.

Example
Delete the entire list:

thislist = ["apple", "banana", "cherry"]
del thislist
Clear the List
The clear() method empties the list.

The list still remains, but it has no content.

Example
Clear the list content:

thislist = ["apple", "banana", "cherry"]
thislist.clear()
print(thislist)

Python - Listas de Loop
Percorrer uma lista
Você pode percorrer os itens da lista usando um for loop:

Exemplo
Imprima todos os itens da lista, um por um:

thislist = ["apple", "banana", "cherry"]
for x in thislist:
  print(x)
Saiba mais sobre forloops em nosso capítulo Python For Loops .

Percorrer os números de índice
Você também pode percorrer os itens da lista consultando seu número de índice.

Use as funções range()e len()para criar um iterável adequado.

Exemplo
Imprima todos os itens consultando seu número de índice:

thislist = ["apple", "banana", "cherry"]
for i in range(len(thislist)):
  print(thislist[i])
O iterável criado no exemplo acima é [0, 1, 2].

PROPAGANDA

Usando um loop while
Você pode percorrer os itens da lista usando um whileloop.

Use a len()função para determinar o comprimento da lista, então comece em 0 e faça um loop pelos itens da lista consultando seus índices.

Lembre-se de aumentar o índice em 1 após cada iteração.

Exemplo
Imprima todos os itens, usando um whileloop para percorrer todos os números de índice

thislist = ["apple", "banana", "cherry"]
i = 0
while i < len(thislist):
  print(thislist[i])
  i = i + 1
Saiba mais sobre whileloops em nosso capítulo Python While Loops .

Loop usando compreensão de lista
O List Comprehension oferece a sintaxe mais curta para percorrer listas:

Exemplo
Um forloop de mão curto que imprimirá todos os itens em uma lista:

thislist = ["apple", "banana", "cherry"]
[print(x) for x in thislist]
Saiba mais sobre compreensão de listas no próximo capítulo: Compreensão de listas .

Python - Compreensão de lista
Compreensão da lista
A compreensão de lista oferece uma sintaxe mais curta quando você deseja criar uma nova lista com base nos valores de uma lista existente.

Exemplo:

Com base em uma lista de frutas, você deseja uma nova lista, contendo apenas as frutas com a letra "a" no nome.

Sem compreensão de lista, você terá que escrever uma fordeclaração com um teste condicional dentro:

Exemplo
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]
newlist = []

for x in fruits:
  if "a" in x:
    newlist.append(x)

print(newlist)
Com compreensão de lista, você pode fazer tudo isso com apenas uma linha de código:

Exemplo
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]

newlist = [x for x in fruits if "a" in x]

print(newlist)
PROPAGANDA

A Sintaxe
newlist = [expression for item in iterable if condition == True]
O valor de retorno é uma nova lista, deixando a lista antiga inalterada.

Doença
A condição é como um filtro que aceita apenas os itens que avaliam como True.

Exemplo
Aceite apenas itens que não sejam "maçã":

newlist = [x for x in fruits if x != "apple"]
A condição if x != "apple"  retornará Truepara todos os elementos exceto "maçã", fazendo com que a nova lista contenha todas as frutas, exceto "maçã".

A condição é opcional e pode ser omitida:

Exemplo
Sem ifdeclaração:

newlist = [x for x in fruits]
Iterável
O iterável pode ser qualquer objeto iterável, como uma lista, tupla, conjunto etc.

Exemplo
Você pode usar a range()função para criar um iterável:

newlist = [x for x in range(10)]
Mesmo exemplo, mas com uma condição:

Exemplo
Aceite apenas números inferiores a 5:

newlist = [x for x in range(10) if x < 5]
Expressão
A expressão é o item atual na iteração, mas também é o resultado, que você pode manipular antes de terminar como um item de lista na nova lista:

Exemplo
Defina os valores na nova lista para maiúsculas:

newlist = [x.upper() for x in fruits]
Você pode definir o resultado para o que quiser:

Exemplo
Defina todos os valores na nova lista para 'hello':

newlist = ['hello' for x in fruits]
A expressão também pode conter condições, não como um filtro, mas como forma de manipular o resultado:

Exemplo
Retorne "laranja" em vez de "banana":

newlist = [x if x != "banana" else "orange" for x in fruits]
A expressão no exemplo acima diz:

"Devolva o item se não for banana, se for banana devolva laranja".

Python - Listas de classificação
Classificar lista alfanumérica
Objetos de lista possuem um sort()método que ordenará a lista de forma alfanumérica, em ordem crescente, por padrão:

Exemplo
Classifique a lista em ordem alfabética:

thislist = ["orange", "mango", "kiwi", "pineapple", "banana"]
thislist.sort()
print(thislist)
Exemplo
Classifique a lista numericamente:

thislist = [100, 50, 65, 82, 23]
thislist.sort()
print(thislist)
Classificação decrescente
Para classificar de forma decrescente, use o argumento de palavra-chave reverse = True:

Exemplo
Ordene a lista decrescente:

thislist = ["orange", "mango", "kiwi", "pineapple", "banana"]
thislist.sort(reverse = True)
print(thislist)
Exemplo
Ordene a lista decrescente:

thislist = [100, 50, 65, 82, 23]
thislist.sort(reverse = True)
print(thislist)
PROPAGANDA

Personalizar a função de classificação
Você também pode personalizar sua própria função usando o argumento de palavra-chave .key = function

A função retornará um número que será usado para ordenar a lista (o número mais baixo primeiro):

Exemplo
Classifique a lista com base em quão próximo o número está de 50:

def myfunc(n):
  return abs(n - 50)

thislist = [100, 50, 65, 82, 23]
thislist.sort(key = myfunc)
print(thislist)
Classificação sem distinção entre maiúsculas e minúsculas
Por padrão, o sort()método diferencia maiúsculas de minúsculas, resultando em todas as letras maiúsculas classificadas antes das minúsculas:

Exemplo
A classificação com distinção entre maiúsculas e minúsculas pode fornecer um resultado inesperado:

thislist = ["banana", "Orange", "Kiwi", "cherry"]
thislist.sort()
print(thislist)
Felizmente, podemos usar funções internas como funções-chave ao classificar uma lista.

Portanto, se você deseja uma função de classificação que não diferencia maiúsculas de minúsculas, use str.lower como uma função de chave:

Exemplo
Execute uma classificação que não diferencia maiúsculas de minúsculas da lista:

thislist = ["banana", "Orange", "Kiwi", "cherry"]
thislist.sort(key = str.lower)
print(thislist)
Ordem reversa
E se você quiser inverter a ordem de uma lista, independentemente do alfabeto?

O reverse()método inverte a ordem de classificação atual dos elementos.

Exemplo
Inverta a ordem dos itens da lista:

thislist = ["banana", "Orange", "Kiwi", "cherry"]
thislist.reverse()
print(thislist)

Python - Copiar listas
Copiar uma lista
Você não pode copiar uma lista simplesmente digitando list2 = list1, porque: list2será apenas uma referência a list1, e as alterações feitas list1automaticamente também serão feitas em list2.

Existem maneiras de fazer uma cópia, uma delas é usar o método List interno copy().

Exemplo
Faça uma cópia de uma lista com o copy()método:

thislist = ["apple", "banana", "cherry"]
mylist = thislist.copy()
print(mylist)
Outra maneira de fazer uma cópia é usar o método interno list().

Exemplo
Faça uma cópia de uma lista com o list()método:

thislist = ["apple", "banana", "cherry"]
mylist = list(thislist)
print(mylist)

Python - Junte-se a listas
Junte-se a duas listas
Existem várias maneiras de unir ou concatenar duas ou mais listas em Python.

Uma das maneiras mais fáceis é usando o + operador.

Exemplo
Junte-se a duas listas:

list1 = ["a", "b", "c"]
list2 = [1, 2, 3]

list3 = list1 + list2
print(list3)
Outra maneira de juntar duas listas é anexando todos os itens da lista2 na lista1, um por um:

Exemplo
Anexar list2 em list1:

list1 = ["a", "b" , "c"]
list2 = [1, 2, 3]

for x in list2:
  list1.append(x)

print(list1)
Ou você pode usar o extend() método, cuja finalidade é adicionar elementos de uma lista para outra lista:

Exemplo
Use o extend()método para adicionar list2 no final de list1:

list1 = ["a", "b" , "c"]
list2 = [1, 2, 3]

list1.extend(list2)
print(list1)

Python - Listar métodos
Listar métodos
Python tem um conjunto de métodos integrados que você pode usar em listas.

Method	Description
append()	Adds an element at the end of the list
clear()	Removes all the elements from the list
copy()	Returns a copy of the list
count()	Returns the number of elements with the specified value
extend()	Add the elements of a list (or any iterable), to the end of the current list
index()	Returns the index of the first element with the specified value
insert()	Adds an element at the specified position
pop()	Removes the element at the specified position
remove()	Removes the item with the specified value
reverse()	Reverses the order of the list
sort()	Sorts the list
