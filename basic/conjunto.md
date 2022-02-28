Conjuntos Python
myset = {"apple", "banana", "cherry"}
Definir
Os conjuntos são usados ​​para armazenar vários itens em uma única variável.

Set é um dos 4 tipos de dados internos do Python usados ​​para armazenar coleções de dados, os outros 3 são List , Tuple e Dictionary , todos com qualidades e usos diferentes.

Um conjunto é uma coleção não ordenada , imutável* e não indexada .

* Nota: Os itens definidos não podem ser alterados, mas você pode remover itens e adicionar novos itens.

Os conjuntos são escritos com colchetes.

Exemplo
Crie um conjunto:

thisset = {"apple", "banana", "cherry"}
print(thisset)
Observação: os conjuntos não são ordenados, portanto, você não pode ter certeza em qual ordem os itens aparecerão.

Definir itens
Os itens do conjunto não são ordenados, não podem ser alterados e não permitem valores duplicados.

Não ordenado
Não ordenado significa que os itens em um conjunto não têm uma ordem definida.

Os itens do conjunto podem aparecer em uma ordem diferente toda vez que você os usa e não podem ser referenciados por índice ou chave.

Imutável
Os itens do conjunto são imutáveis, o que significa que não podemos alterar os itens após a criação do conjunto.

Depois que um conjunto é criado, você não pode alterar seus itens, mas pode remover itens e adicionar novos itens.

Duplicatas não permitidas
Os conjuntos não podem ter dois itens com o mesmo valor.

Exemplo
Valores duplicados serão ignorados:

thisset = {"apple", "banana", "cherry", "apple"}

print(thisset)

Python - Acessar Itens do Conjunto
Acessar itens
Você não pode acessar itens em um conjunto fazendo referência a um índice ou a uma chave.

Mas você pode percorrer os itens do conjunto usando um for loop ou perguntar se um valor especificado está presente em um conjunto, usando a palavra- inchave.

Exemplo
Percorra o conjunto e imprima os valores:

thisset = {"apple", "banana", "cherry"}

for x in thisset:
  print(x)
Exemplo
Verifique se "banana" está presente no conjunto:

thisset = {"apple", "banana", "cherry"}

print("banana" in thisset)
Alterar itens
Depois que um conjunto é criado, você não pode alterar seus itens, mas pode adicionar novos itens.

Python - Adicionar itens de conjunto
Adicionar itens
Depois que um conjunto é criado, você não pode alterar seus itens, mas pode adicionar novos itens.

Para adicionar um item a um conjunto, use o add() método.

Exemplo
Adicione um item a um conjunto, usando o add() método:

thisset = {"apple", "banana", "cherry"}

thisset.add("orange")

print(thisset)
Adicionar conjuntos
Para adicionar itens de outro conjunto ao conjunto atual, use o update() método.

Exemplo
Adicione elementos de tropicalinto thisset:

thisset = {"apple", "banana", "cherry"}
tropical = {"pineapple", "mango", "papaya"}

thisset.update(tropical)

print(thisset)
Adicionar qualquer iterável
O objeto no update()método não precisa ser um conjunto, pode ser qualquer objeto iterável (tuplas, listas, dicionários etc.).

Exemplo
Adicione elementos de uma lista a at set:

thisset = {"apple", "banana", "cherry"}
mylist = ["kiwi", "orange"]

thisset.update(mylist)

print(thisset)

Python - Remover itens do conjunto
Remover item
Para remover um item em um conjunto, use o método remove(), ou .discard()

Exemplo
Remova "banana" usando o remove() método:

thisset = {"apple", "banana", "cherry"}

thisset.remove("banana")

print(thisset)
Nota: Se o item a ser removido não existir, remove()será gerado um erro.

Exemplo
Remova "banana" usando o discard() método:

thisset = {"apple", "banana", "cherry"}

thisset.discard("banana")

print(thisset)
Nota: Se o item a ser removido não existir, NÃOdiscard() irá gerar um erro.

Você também pode usar o pop()método para remover um item, mas esse método removerá o último item. Lembre-se de que os conjuntos não são ordenados, então você não saberá qual item será removido.

O valor de retorno do pop()método é o item removido.

Exemplo
Remova o último item usando o pop() método:

thisset = {"apple", "banana", "cherry"}

x = thisset.pop()

print(x)

print(thisset)
Nota: Os conjuntos não são ordenados , portanto, ao usar o pop()método, você não sabe qual item será removido.

Exemplo
O clear() método esvazia o conjunto:

thisset = {"apple", "banana", "cherry"}

thisset.clear()

print(thisset)
Exemplo
A delpalavra-chave excluirá o conjunto completamente:

thisset = {"apple", "banana", "cherry"}

del thisset

print(thisset)

Python - Conjuntos de Loops
Itens de loop
Você pode percorrer os itens definidos usando um for loop:

Exemplo
Percorra o conjunto e imprima os valores:

thisset = {"apple", "banana", "cherry"}

for x in thisset:
  print(x)

Python - Conjuntos de junção
Junte dois conjuntos
Existem várias maneiras de unir dois ou mais conjuntos em Python.

Você pode usar o union()método que retorna um novo conjunto contendo todos os itens de ambos os conjuntos ou o update()método que insere todos os itens de um conjunto em outro:

Exemplo
O union()método retorna um novo conjunto com todos os itens de ambos os conjuntos:

set1 = {"a", "b" , "c"}
set2 = {1, 2, 3}

set3 = set1.union(set2)
print(set3)
Exemplo
O update()método insere os itens em set2 em set1:

set1 = {"a", "b" , "c"}
set2 = {1, 2, 3}

set1.update(set2)
print(set1)
Nota: Ambos union()e update() excluirão quaisquer itens duplicados.

PROPAGANDA

Mantenha APENAS as duplicatas
O intersection_update()método manterá apenas os itens presentes em ambos os conjuntos.

Exemplo
Mantenha os itens que existem em ambos set x, e set y:

x = {"apple", "banana", "cherry"}
y = {"google", "microsoft", "apple"}

x.intersection_update(y)

print(x)
O intersection()método retornará um novo conjunto, que contém apenas os itens presentes em ambos os conjuntos.

Exemplo
Retorna um set que contém os itens que existem em set xe set y:

x = {"apple", "banana", "cherry"}
y = {"google", "microsoft", "apple"}

z = x.intersection(y)

print(z)
Mantenha tudo, mas não as duplicatas
O symmetric_difference_update()método manterá apenas os elementos que NÃO estão presentes em ambos os conjuntos.

Exemplo
Guarde os itens que não estão presentes em ambos os conjuntos:

x = {"apple", "banana", "cherry"}
y = {"google", "microsoft", "apple"}

x.symmetric_difference_update(y)

print(x)
O symmetric_difference()método retornará um novo conjunto, que contém apenas os elementos que NÃO estão presentes em ambos os conjuntos.

Exemplo
Retorna um conjunto que contém todos os itens de ambos os conjuntos, exceto os itens presentes em ambos:

x = {"apple", "banana", "cherry"}
y = {"google", "microsoft", "apple"}

z = x.symmetric_difference(y)

print(z)

Python - Definir métodos
Definir métodos
Python tem um conjunto de métodos integrados que você pode usar em conjuntos.

Method	Description
add()	Adds an element to the set
clear()	Removes all the elements from the set
copy()	Returns a copy of the set
difference()	Returns a set containing the difference between two or more sets
difference_update()	Removes the items in this set that are also included in another, specified set
discard()	Remove the specified item
intersection()	Returns a set, that is the intersection of two other sets
intersection_update()	Removes the items in this set that are not present in other, specified set(s)
isdisjoint()	Returns whether two sets have a intersection or not
issubset()	Returns whether another set contains this set or not
issuperset()	Returns whether this set contains another set or not
pop()	Removes an element from the set
remove()	Removes the specified element
symmetric_difference()	Returns a set with the symmetric differences of two sets
symmetric_difference_update()	inserts the symmetric differences from this set and another
union()	Return a set containing the union of sets
update()	Update the set with the union of this set and others

