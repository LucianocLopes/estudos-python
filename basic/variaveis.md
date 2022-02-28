Variáveis ​​Python
Varia b l e s
Variáveis ​​são contêineres para armazenar valores de dados.

Criando variáveis
Python não tem comando para declarar uma variável.

Uma variável é criada no momento em que você atribui um valor a ela.

Exemplo
x = 5
y = "John"
print(x)
print(y)
As variáveis ​​não precisam ser declaradas com nenhum tipo específico e podem até mudar de tipo depois de terem sido definidas.

Exemplo
x = 4       # x is of type int
x = "Sally" # x is now of type str
print(x)
Fundição
Se você deseja especificar o tipo de dados de uma variável, isso pode ser feito com conversão.

Exemplo
x = str(3)    # x will be '3'
y = int(3)    # y will be 3
z = float(3)  # z will be 3.0

Obter o tipo
Você pode obter o tipo de dados de uma variável com a type()função.

Exemplo
x = 5
y = "John"
print(type(x))
print(type(y))
Você aprenderá mais sobre tipos de dados e transmissão posteriormente neste tutorial.
Citações simples ou duplas?
Variáveis ​​de string podem ser declaradas usando aspas simples ou duplas:

Exemplo
x = "John"
# is the same as
x = 'John'
Maiúsculas e Minúsculas
Os nomes de variáveis ​​diferenciam maiúsculas de minúsculas.

Exemplo
Isso criará duas variáveis:

a = 4
A = "Sally"
#A will not overwrite a

Python - Nomes de Variáveis
Nomes de Variáveis
Uma variável pode ter um nome curto (como x e y) ou um nome mais descritivo (age, carname, total_volume). Regras para variáveis ​​Python:
Um nome de variável deve começar com uma letra ou o caractere sublinhado
Um nome de variável não pode começar com um número
Um nome de variável pode conter apenas caracteres alfanuméricos e sublinhados (Az, 0-9 e _ )
Os nomes das variáveis ​​diferenciam maiúsculas de minúsculas (idade, idade e IDADE são três variáveis ​​diferentes)
Exemplo
Nomes de variáveis ​​legais:

myvar = "John"
my_var = "John"
_my_var = "John"
myVar = "John"
MYVAR = "John"
myvar2 = "John"
Exemplo
Nomes de variáveis ​​ilegais:

2myvar = "John"
my-var = "John"
my var = "John"
Lembre-se de que os nomes das variáveis ​​diferenciam maiúsculas de minúsculasPython - Variable Names
Variable Names
A variable can have a short name (like x and y) or a more descriptive name (age, carname, total_volume). Rules for Python variables:
A variable name must start with a letter or the underscore character
A variable name cannot start with a number
A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )
Variable names are case-sensitive (age, Age and AGE are three different variables)
Example
Legal variable names:

myvar = "John"
my_var = "John"
_my_var = "John"
myVar = "John"
MYVAR = "John"
myvar2 = "John"
Example
Illegal variable names:

2myvar = "John"
my-var = "John"
my var = "John"
Remember that variable names are case-sensitive

Nomes de variáveis ​​de várias palavras
Nomes de variáveis ​​com mais de uma palavra podem ser difíceis de ler.

Existem várias técnicas que você pode usar para torná-los mais legíveis:

Caixa de camelo
Cada palavra, exceto a primeira, começa com letra maiúscula:

myVariableName = "John"
Caso Pascal
Cada palavra começa com uma letra maiúscula:

MyVariableName = "John"
Caso da Cobra
Cada palavra é separada por um caractere de sublinhado:

my_variable_name = "John"

Variáveis ​​Python - Atribuir vários valores
Muitos valores para múltiplas variáveis
Python permite atribuir valores a várias variáveis ​​em uma linha:

Exemplo
x, y, z = "Orange", "Banana", "Cherry"
print(x)
print(y)
print(z)
Nota: Certifique-se de que o número de variáveis ​​corresponda ao número de valores, caso contrário você receberá um erro.

Um valor para várias variáveis
E você pode atribuir o mesmo valor a várias variáveis ​​em uma linha:

Exemplo
x = y = z = "Orange"
print(x)
print(y)
print(z)
Descompactar uma coleção
Se você tem uma coleção de valores em uma lista, tupla etc. Python permite que você extraia os valores em variáveis. Isso é chamado de descompactação .

Exemplo
Descompacte uma lista:

fruits = ["apple", "banana", "cherry"]
x, y, z = fruits
print(x)
print(y)
print(z)
Saiba mais sobre como descompactar em nosso capítulo Descompactar Tuplas .****

Python - Variáveis ​​de saída
Variáveis ​​de saída
A instrução Python printé frequentemente usada para gerar variáveis.

Para combinar texto e uma variável, o Python usa o +caractere:

Exemplo
x = "awesome"
print("Python is " + x)
Você também pode usar o +caractere para adicionar uma variável a outra variável:

Exemplo
x = "Python is "
y = "awesome"
z =  x + y
print(z)
Para números, o +caractere funciona como um operador matemático:

Exemplo
x = 5
y = 10
print(x + y)
Se você tentar combinar uma string e um número, o Python lhe dará um erro:

Exemplo
x = 5
y = "John"
print(x + y)

Python - Variáveis ​​Globais
Variáveis ​​globais
Variáveis ​​criadas fora de uma função (como em todos os exemplos acima) são conhecidas como variáveis ​​globais.

As variáveis ​​globais podem ser usadas por todos, tanto dentro das funções quanto fora delas.

Exemplo
Crie uma variável fora de uma função e use-a dentro da função

x = "awesome"

def myfunc():
  print("Python is " + x)

myfunc()
Se você criar uma variável com o mesmo nome dentro de uma função, essa variável será local e só poderá ser usada dentro da função. A variável global com o mesmo nome permanecerá como estava, global e com o valor original.

Exemplo
Crie uma variável dentro de uma função, com o mesmo nome da variável global

x = "awesome"

def myfunc():
  x = "fantastic"
  print("Python is " + x)

myfunc()

print("Python is " + x)

A palavra-chave global
Normalmente, quando você cria uma variável dentro de uma função, essa variável é local e só pode ser usada dentro dessa função.

Para criar uma variável global dentro de uma função, você pode usar a palavra- globalchave.

Exemplo
Se você usar a palavra- globalchave, a variável pertence ao escopo global:

def myfunc():
  global x
  x = "fantastic"

myfunc()

print("Python is " + x)
Além disso, use a palavra- globalchave se quiser alterar uma variável global dentro de uma função.

Exemplo
Para alterar o valor de uma variável global dentro de uma função, consulte a variável usando a globalpalavra-chave:

x = "awesome"

def myfunc():
  global x
  x = "fantastic"

myfunc()

print("Python is " + x)
