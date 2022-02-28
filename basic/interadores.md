Iteradores Python
Iteradores Python
Um iterador é um objeto que contém um número contável de valores.

Um iterador é um objeto que pode ser iterado, o que significa que você pode percorrer todos os valores.

Tecnicamente, em Python, um iterador é um objeto que implementa o protocolo do iterador, que consiste nos métodos __iter__() e __next__().

Iterador vs Iterável
Listas, tuplas, dicionários e conjuntos são todos objetos iteráveis. Eles são contêineres iteráveis ​​dos quais você pode obter um iterador.

Todos esses objetos têm um iter()método que é usado para obter um iterador:

Exemplo
Retorne um iterador de uma tupla e imprima cada valor:

mytuple = ("apple", "banana", "cherry")
myit = iter(mytuple)

print(next(myit))
print(next(myit))
print(next(myit))
Mesmo strings são objetos iteráveis ​​e podem retornar um iterador:

Exemplo
Strings também são objetos iteráveis, contendo uma sequência de caracteres:

mystr = "banana"
myit = iter(mystr)

print(next(myit))
print(next(myit))
print(next(myit))
print(next(myit))
print(next(myit))
print(next(myit))
Fazendo um loop através de um iterador
Também podemos usar um forloop para iterar através de um objeto iterável:

Exemplo
Iterar os valores de uma tupla:

mytuple = ("apple", "banana", "cherry")

for x in mytuple:
  print(x)
Exemplo
Iterar os caracteres de uma string:

mystr = "banana"

for x in mystr:
  print(x)
O forloop na verdade cria um objeto iterador e executa o método next() para cada loop.

PROPAGANDA

Criar um iterador
Para criar um objeto/classe como um iterador, você precisa implementar os métodos __iter__()e __next__()seu objeto.

Como você aprendeu no capítulo Classes/Objetos do Python , todas as classes têm uma função chamada __init__(), que permite que você inicialize quando o objeto estiver sendo criado.

O __iter__()método age de forma semelhante, você pode fazer operações (inicialização etc.), mas deve sempre retornar o próprio objeto iterador.

O __next__()método também permite fazer operações, devendo retornar o próximo item na sequência.

Exemplo
Crie um iterador que retorne números, começando com 1, e cada sequência aumentará em um (retornando 1,2,3,4,5 etc.):

class MyNumbers:
  def __iter__(self):
    self.a = 1
    return self

  def __next__(self):
    x = self.a
    self.a += 1
    return x

myclass = MyNumbers()
myiter = iter(myclass)

print(next(myiter))
print(next(myiter))
print(next(myiter))
print(next(myiter))
print(next(myiter))
Parar Iteração
O exemplo acima continuaria para sempre se você tivesse instruções next() suficientes ou se fosse usado em um forloop.

Para evitar que a iteração continue para sempre, podemos usar a StopIterationinstrução.

No __next__()método, podemos adicionar uma condição de término para gerar um erro se a iteração for feita um número especificado de vezes:

Exemplo
Pare após 20 iterações:

class MyNumbers:
  def __iter__(self):
    self.a = 1
    return self

  def __next__(self):
    if self.a <= 20:
      x = self.a
      self.a += 1
      return x
    else:
      raise StopIteration

myclass = MyNumbers()
myiter = iter(myclass)

for x in myiter:
  print(x)