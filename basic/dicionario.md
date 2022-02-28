Dicionários Python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
Dicionário
Os dicionários são usados ​​para armazenar valores de dados em pares chave:valor.

Um dicionário é uma coleção ordenada*, mutável e que não permite duplicatas.

A partir da versão 3.7 do Python, os dicionários são ordenados . No Python 3.6 e anteriores, os dicionários não são ordenados .

Os dicionários são escritos com colchetes e possuem chaves e valores:

Exemplo
Crie e imprima um dicionário:

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict)
Itens do dicionário
Os itens do dicionário são ordenados, alteráveis ​​e não permitem duplicatas.

Os itens do dicionário são apresentados em pares chave:valor e podem ser referenciados usando o nome da chave.

Exemplo
Imprima o valor "marca" do dicionário:

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict["brand"])
Ordenado ou Não Ordenado?
A partir da versão 3.7 do Python, os dicionários são ordenados . No Python 3.6 e anteriores, os dicionários não são ordenados .

Quando dizemos que os dicionários estão ordenados, significa que os itens têm uma ordem definida, e essa ordem não será alterada.

Não ordenado significa que os itens não têm uma ordem definida, você não pode fazer referência a um item usando um índice.

Mutável
Os dicionários são mutáveis, o que significa que podemos alterar, adicionar ou remover itens após a criação do dicionário.

Duplicatas não permitidas
Os dicionários não podem ter dois itens com a mesma chave:

Exemplo
Valores duplicados substituirão os valores existentes:

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964,
  "year": 2020
}
print(thisdict)
PROPAGANDA

Tamanho do dicionário
Para determinar quantos itens um dicionário possui, use a len()função:

Exemplo
Imprima o número de itens no dicionário:

print(len(thisdict))
Itens do Dicionário - Tipos de Dados
Os valores nos itens do dicionário podem ser de qualquer tipo de dados:

Exemplo
Tipos de dados String, int, boolean e list:

thisdict = {
  "brand": "Ford",
  "electric": False,
  "year": 1964,
  "colors": ["red", "white", "blue"]
}
tipo()
Da perspectiva do Python, os dicionários são definidos como objetos com o tipo de dados 'dict':

<class 'dict'>
Exemplo
Imprima o tipo de dados de um dicionário:

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(type(thisdict))
Coleções Python (matrizes)
Existem quatro tipos de dados de coleção na linguagem de programação Python:

Lista é uma coleção que é ordenada e mutável. Permite membros duplicados.
Tupla é uma coleção ordenada e imutável. Permite membros duplicados.
Set é uma coleção não ordenada, imutável* e não indexada. Nenhum membro duplicado.
Dicionário é uma coleção ordenada** e mutável. Nenhum membro duplicado.
*Os itens do conjunto são imutáveis, mas você pode remover e/ou adicionar itens sempre que quiser.

**A partir da versão 3.7 do Python, os dicionários são ordenados . No Python 3.6 e anteriores, os dicionários não são ordenados .

Ao escolher um tipo de coleção, é útil entender as propriedades desse tipo. Escolher o tipo certo para um determinado conjunto de dados pode significar retenção de significado e pode significar um aumento na eficiência ou segurança.

Python - Acessar itens do dicionário
Acessando itens
Você pode acessar os itens de um dicionário consultando o nome da chave, entre colchetes:

Exemplo
Obtenha o valor da chave "model":

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
x = thisdict["model"]
Existe também um método chamado get()que lhe dará o mesmo resultado:

Exemplo
Obtenha o valor da chave "model":

x = thisdict.get("model")
Obter chaves
O keys()método retornará uma lista de todas as chaves do dicionário.

Exemplo
Obtenha uma lista das chaves:

x = thisdict.keys()
A lista de chaves é uma visualização do dicionário, o que significa que quaisquer alterações feitas no dicionário serão refletidas na lista de chaves.

Exemplo
Adicione um novo item ao dicionário original e veja se a lista de chaves também é atualizada:

car = {
"brand": "Ford",
"model": "Mustang",
"year": 1964
}

x = car.keys()

print(x) #before the change

car["color"] = "white"

print(x) #after the change
PROPAGANDA

Obter valores
O values()método retornará uma lista de todos os valores do dicionário.

Exemplo
Obtenha uma lista dos valores:

x = thisdict.values()
A lista de valores é uma visualização do dicionário, o que significa que quaisquer alterações feitas no dicionário serão refletidas na lista de valores.

Exemplo
Faça uma alteração no dicionário original e veja se a lista de valores também é atualizada:

car = {
"brand": "Ford",
"model": "Mustang",
"year": 1964
}

x = car.values()

print(x) #before the change

car["year"] = 2020

print(x) #after the change
Exemplo
Adicione um novo item ao dicionário original e veja se a lista de valores também é atualizada:

car = {
"brand": "Ford",
"model": "Mustang",
"year": 1964
}

x = car.values()

print(x) #before the change

car["color"] = "red"

print(x) #after the change
Obter itens
O items()método retornará cada item em um dicionário, como tuplas em uma lista.

Exemplo
Obter uma lista dos pares chave:valor

x = thisdict.items()
A lista retornada é uma visualização dos itens do dicionário, o que significa que quaisquer alterações feitas no dicionário serão refletidas na lista de itens.

Exemplo
Faça uma alteração no dicionário original e veja se a lista de itens também é atualizada:

car = {
"brand": "Ford",
"model": "Mustang",
"year": 1964
}

x = car.items()

print(x) #before the change

car["year"] = 2020

print(x) #after the change
Exemplo
Adicione um novo item ao dicionário original e veja se a lista de itens também é atualizada:

car = {
"brand": "Ford",
"model": "Mustang",
"year": 1964
}

x = car.items()

print(x) #before the change

car["color"] = "red"

print(x) #after the change
Verifique se a chave existe
Para determinar se uma chave especificada está presente em um dicionário, use a inpalavra-chave:

Exemplo
Verifique se "modelo" está presente no dicionário:

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
if "model" in thisdict:
  print("Yes, 'model' is one of the keys in the thisdict dictionary")

Python - Alterar itens do dicionário
Mudar valores
Você pode alterar o valor de um item específico consultando seu nome de chave:

Exemplo
Altere o "ano" para 2018:

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict["year"] = 2018
Atualizar dicionário
O update()método atualizará o dicionário com os itens do argumento fornecido.

O argumento deve ser um dicionário ou um objeto iterável com pares chave:valor.

Exemplo
Atualize o "ano" do carro usando o update() método:

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict.update({"year": 2020})

Python - Adicionar itens de dicionário
Adicionando itens
A adição de um item ao dicionário é feita usando uma nova chave de índice e atribuindo um valor a ela:

Exemplo
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict["color"] = "red"
print(thisdict)
Atualizar dicionário
O update()método atualizará o dicionário com os itens de um determinado argumento. Se o item não existir, o item será adicionado.

O argumento deve ser um dicionário ou um objeto iterável com pares chave:valor.

Exemplo
Adicione um item de cor ao dicionário usando o update() método:

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict.update({"color": "red"})

Python - Remover itens do dicionário
Removendo itens
Existem vários métodos para remover itens de um dicionário:

Exemplo
O pop()método remove o item com o nome de chave especificado:

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict.pop("model")
print(thisdict)
Exemplo
O popitem()método remove o último item inserido (nas versões anteriores à 3.7, um item aleatório é removido):

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict.popitem()
print(thisdict)
Exemplo
A delpalavra-chave remove o item com o nome de chave especificado:

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
del thisdict["model"]
print(thisdict)
Exemplo
A delpalavra-chave também pode excluir completamente o dicionário:

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
del thisdict
print(thisdict) #this will cause an error because "thisdict" no longer exists.
Exemplo
O clear()método esvazia o dicionário:

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
thisdict.clear()
print(thisdict)

Python - Dicionários de loop
Percorrer um dicionário
Você pode percorrer um dicionário usando um forloop.

Ao percorrer um dicionário, o valor de retorno são as chaves do dicionário, mas também existem métodos para retornar os valores .

Exemplo
Imprima todos os nomes de chave no dicionário, um por um:

for x in thisdict:
  print(x)
Exemplo
Imprima todos os valores no dicionário, um por um:

for x in thisdict:
  print(thisdict[x])
Exemplo
Você também pode usar o values()método para retornar valores de um dicionário:

for x in thisdict.values():
  print(x)
Exemplo
Você pode usar o keys()método para retornar as chaves de um dicionário:

for x in thisdict.keys():
  print(x)
Exemplo
Faça um loop pelas chaves e valores , usando o items()método:

for x, y in thisdict.items():
  print(x, y)

Python - Copiar dicionários
Copiar um dicionário
Você não pode copiar um dicionário simplesmente digitando dict2 = dict1, porque: dict2será apenas uma referência a dict1, e as alterações feitas em dict1serão feitas automaticamente também em dict2.

Existem maneiras de fazer uma cópia, uma delas é usar o método interno do Dicionário copy().

Exemplo
Faça uma cópia de um dicionário com o copy()método:

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
mydict = thisdict.copy()
print(mydict)
Outra maneira de fazer uma cópia é usar a função interna dict().

Exemplo
Faça uma cópia de um dicionário com a dict() função:

thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
mydict = dict(thisdict)
print(mydict)

Python - Dicionários aninhados
Dicionários aninhados
Um dicionário pode conter dicionários, isso é chamado de dicionários aninhados.

Exemplo
Crie um dicionário que contenha três dicionários:

myfamily = {
  "child1" : {
    "name" : "Emil",
    "year" : 2004
  },
  "child2" : {
    "name" : "Tobias",
    "year" : 2007
  },
  "child3" : {
    "name" : "Linus",
    "year" : 2011
  }
}
Ou, se você quiser adicionar três dicionários em um novo dicionário:

Exemplo
Crie três dicionários e, em seguida, crie um dicionário que conterá os outros três dicionários:

child1 = {
  "name" : "Emil",
  "year" : 2004
}
child2 = {
  "name" : "Tobias",
  "year" : 2007
}
child3 = {
  "name" : "Linus",
  "year" : 2011
}

myfamily = {
  "child1" : child1,
  "child2" : child2,
  "child3" : child3
}

Métodos de dicionário Python
Métodos de dicionário
Python tem um conjunto de métodos integrados que você pode usar em dicionários.

Method	Description
clear()	Removes all the elements from the dictionary
copy()	Returns a copy of the dictionary
fromkeys()	Returns a dictionary with the specified keys and value
get()	Returns the value of the specified key
items()	Returns a list containing a tuple for each key value pair
keys()	Returns a list containing the dictionary's keys
pop()	Removes the element with the specified key
popitem()	Removes the last inserted key-value pair
setdefault()	Returns the value of the specified key. If the key does not exist: insert the key, with the specified value
update()	Updates the dictionary with the specified key-value pairs
values()	Returns a list of all the values in the dictionary
