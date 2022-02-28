Classes e objetos Python
Classes/objetos Python
Python é uma linguagem de programação orientada a objetos.

Quase tudo em Python é um objeto, com suas propriedades e métodos.

Uma classe é como um construtor de objetos, ou um "projeto" para criar objetos.

Criar uma classe
Para criar uma classe, use a palavra-chave class:

Exemplo
Crie uma classe chamada MyClass, com uma propriedade chamada x:

class MyClass:
  x = 5
Criar objeto
Agora podemos usar a classe chamada MyClass para criar objetos:

Exemplo
Crie um objeto chamado p1 e imprima o valor de x:

p1 = MyClass()
print(p1.x)
A função __init__()
Os exemplos acima são classes e objetos em sua forma mais simples e não são realmente úteis em aplicações da vida real.

Para entender o significado das classes, temos que entender a função __init__() embutida.

Todas as classes possuem uma função chamada __init__(), que sempre é executada quando a classe está sendo iniciada.

Use a função __init__() para atribuir valores às propriedades do objeto ou outras operações que são necessárias quando o objeto está sendo criado:

Exemplo
Crie uma classe chamada Person, use a função __init__() para atribuir valores para nome e idade:

class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

p1 = Person("John", 36)

print(p1.name)
print(p1.age)
Nota: A __init__()função é chamada automaticamente toda vez que a classe está sendo usada para criar um novo objeto.

PROPAGANDA

Métodos de objeto
Objetos também podem conter métodos. Métodos em objetos são funções que pertencem ao objeto.

Vamos criar um método na classe Person:

Exemplo
Insira uma função que imprima uma saudação e execute-a no objeto p1:

class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

  def myfunc(self):
    print("Hello my name is " + self.name)

p1 = Person("John", 36)
p1.myfunc()
Nota: O selfparâmetro é uma referência à instância atual da classe e é usado para acessar variáveis ​​que pertencem à classe.

O parâmetro self
O selfparâmetro é uma referência à instância atual da classe e é usado para acessar as variáveis ​​que pertencem à classe.

Ele não precisa ser nomeado self, você pode chamá-lo como quiser, mas deve ser o primeiro parâmetro de qualquer função da classe:

Exemplo
Use as palavras mysillyobject e abc em vez de self :

class Person:
  def __init__(mysillyobject, name, age):
    mysillyobject.name = name
    mysillyobject.age = age

  def myfunc(abc):
    print("Hello my name is " + abc.name)

p1 = Person("John", 36)
p1.myfunc()
Modificar propriedades do objeto
Você pode modificar propriedades em objetos como este:

Exemplo
Defina a idade de p1 para 40:

p1.age = 40
Excluir propriedades do objeto
Você pode excluir propriedades em objetos usando a delpalavra-chave:

Exemplo
Exclua a propriedade age do objeto p1:

del p1.age
Excluir objetos
Você pode excluir objetos usando a delpalavra-chave:

Exemplo
Exclua o objeto p1:

del p1
A declaração de passagem
classAs definições não podem estar vazias, mas se por algum motivo você tiver uma classdefinição sem conteúdo, coloque a passdeclaração para evitar erros.

Exemplo
class Person:
  pass
