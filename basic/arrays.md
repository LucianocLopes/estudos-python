# Matrizes (Arrays) Python
Nota: O Python não possui suporte integrado para Arrays, mas as Listas do Python podem ser usadas.

**Matrizes**
Nota: Esta página mostra como usar LISTS como ARRAYS, porém, para trabalhar com arrays em Python você terá que importar uma biblioteca, como a biblioteca NumPy .
Arrays são usados ​​para armazenar vários valores em uma única variável:
Exemplo
Crie um array contendo nomes de carros:

```py
cars = ["Ford", "Volvo", "BMW"]
```

**O que é uma Matriz?**
Um array é uma variável especial, que pode conter mais de um valor por vez.
Se você tiver uma lista de itens (uma lista de nomes de carros, por exemplo), armazenar os carros em variáveis ​​únicas pode ficar assim:

```py
car1 = "Ford"
car2 = "Volvo"
car3 = "BMW"
```

No entanto, e se você quiser percorrer os carros e encontrar um específico? E se você não tivesse 3 carros, mas 300?
A solução é uma matriz!
Uma matriz pode conter muitos valores em um único nome e você pode acessar os valores referindo-se a um número de índice.
Acesse os elementos de um array
Você se refere a um elemento de array referindo-se ao número do índice .
Exemplo
Obtenha o valor do primeiro item da matriz:

```py
x = cars[0]
```

Exemplo
Modifique o valor do primeiro item da matriz:
`cars[0] = "Toyota"`
O comprimento de uma matriz
Use o método len() para retornar o comprimento de uma matriz (o número de elementos em uma matriz).
Exemplo
Retorna o número de elementos no cars array:
`x = len(cars)`
Nota: O comprimento de uma matriz é sempre um a mais do que o índice de matriz mais alto.

**Elementos de Matriz em Loop**
Você pode usar o for inloop para percorrer todos os elementos de uma matriz.
Exemplo
Imprima cada item na carsmatriz:

```py
for x in cars:
  print(x)
```

**Adicionando elementos de matriz**
Você pode usar o método append() para adicionar um elemento a uma matriz.
Exemplo
Adicione mais um elemento ao array cars:
`cars.append("Honda")`

**Removendo elementos da matriz**
Você pode usar o pop()método para remover um elemento da matriz.
Exemplo
Exclua o segundo elemento da matriz cars:
`cars.pop(1)`

Você também pode usar o método remove() para remover um elemento da matriz.
Exemplo
Exclua o elemento que tem o valor "Volvo":
`cars.remove("Volvo")`

Nota: O método remove() da lista remove apenas a primeira ocorrência do valor especificado.

**Métodos de matriz**
Python tem um conjunto de métodos embutidos que você pode usar em listas/matrizes.

| Method | Description |
| :---: | :----------- |
| append() | Adds an element at the end of the list |
| clear() | Removes all the elements from the list |
| copy() | Returns a copy of the list |
| count() | Returns the number of elements with the specified value |
| extend() | Add the elements of a list (or any iterable), to the end of the current list |
| index() | Returns the index of the first element with the specified value |
| insert() | Adds an element at the specified position |
| pop() | Removes the element at the specified position |
| remove() | Removes the first item with the specified value |
| reverse() | Reverses the order of the list |
| sort() | Sorts the list |