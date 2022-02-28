Herança Python
Herança Python
A herança nos permite definir uma classe que herda todos os métodos e propriedades de outra classe.

A classe pai é a classe que está sendo herdada, também chamada de classe base.

A classe filha é a classe que herda de outra classe, também chamada de classe derivada.

Criar uma classe pai
Qualquer classe pode ser uma classe pai, então a sintaxe é a mesma da criação de qualquer outra classe:

Exemplo
Crie uma classe chamada Person, with firstnameand lastnameproperties e um printnamemétodo:

class Person:
  def __init__(self, fname, lname):
    self.firstname = fname
    self.lastname = lname

  def printname(self):
    print(self.firstname, self.lastname)

#Use the Person class to create an object, and then execute the printname method:

x = Person("John", "Doe")
x.printname()
Criar uma classe filha
Para criar uma classe que herde a funcionalidade de outra classe, envie a classe pai como parâmetro ao criar a classe filha:

Exemplo
Crie uma classe chamada Student, que herdará as propriedades e métodos da Personclasse:

class Student(Person):
  pass
Observação: use a palavra- pass chave quando não desejar adicionar outras propriedades ou métodos à classe.

Agora a classe Student tem as mesmas propriedades e métodos que a classe Person.

Exemplo
Use a Studentclasse para criar um objeto e execute o printnamemétodo:

x = Student("Mike", "Olsen")
x.printname()
PROPAGANDA

Adicione a função __init__()
Até agora criamos uma classe filha que herda as propriedades e métodos de seu pai.

Queremos adicionar a __init__()função à classe filha (em vez da palavra- passchave).

Nota: A __init__()função é chamada automaticamente toda vez que a classe está sendo usada para criar um novo objeto.

Exemplo
Adicione a __init__()função à Studentclasse:

class Student(Person):
  def __init__(self, fname, lname):
    #add properties etc.
Quando você adiciona a __init__()função, a classe filha não herdará mais a __init__()função do pai.

Nota: A __init__() função do filho substitui a herança da __init__()função do pai.

Para manter a herança da __init__() função do pai, adicione uma chamada à __init__()função do pai:

Exemplo
class Student(Person):
  def __init__(self, fname, lname):
    Person.__init__(self, fname, lname)
Agora adicionamos com sucesso a função __init__() e mantivemos a herança da classe pai, e estamos prontos para adicionar funcionalidade na __init__()função.

Use a função super()
Python também tem uma super()função que fará com que a classe filha herde todos os métodos e propriedades de seu pai:

Exemplo
class Student(Person):
  def __init__(self, fname, lname):
    super().__init__(fname, lname)
Ao usar a super()função, você não precisa usar o nome do elemento pai, ele herdará automaticamente os métodos e propriedades de seu pai.

Adicionar propriedades
Exemplo
Adicione uma propriedade chamada graduationyearà Studentclasse:

class Student(Person):
  def __init__(self, fname, lname):
    super().__init__(fname, lname)
    self.graduationyear = 2019
No exemplo abaixo, o ano 2019deve ser uma variável e passado para a Studentclasse ao criar objetos de aluno. Para isso, adicione outro parâmetro na função __init__():

Exemplo
Adicione um yearparâmetro e passe o ano correto ao criar objetos:

class Student(Person):
  def __init__(self, fname, lname, year):
    super().__init__(fname, lname)
    self.graduationyear = year

x = Student("Mike", "Olsen", 2019)
Adicionar métodos
Exemplo
Adicione um método chamado welcomeà Studentclasse:

class Student(Person):
  def __init__(self, fname, lname, year):
    super().__init__(fname, lname)
    self.graduationyear = year

  def welcome(self):
    print("Welcome", self.firstname, self.lastname, "to the class of", self.graduationyear)
Se você adicionar um método na classe filha com o mesmo nome de uma função na classe pai, a herança do método pai será substituída.