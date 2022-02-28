Funções do Python
Uma função é um bloco de código que só é executado quando é chamado.

Você pode passar dados, conhecidos como parâmetros, para uma função.

Uma função pode retornar dados como resultado.

Criando uma função
Em Python, uma função é definida usando a palavra-chave def :

Exemplo
def my_function():
  print("Hello from a function")
Chamando uma função
Para chamar uma função, use o nome da função seguido de parênteses:

Exemplo
def my_function():
  print("Hello from a function")

my_function()
Argumentos
As informações podem ser passadas para funções como argumentos.

Os argumentos são especificados após o nome da função, dentro dos parênteses. Você pode adicionar quantos argumentos quiser, basta separá-los com uma vírgula.

O exemplo a seguir tem uma função com um argumento (fname). Quando a função é chamada, passamos um primeiro nome, que é usado dentro da função para imprimir o nome completo:

Exemplo
def my_function(fname):
  print(fname + " Refsnes")

my_function("Emil")
my_function("Tobias")
my_function("Linus")
Os argumentos geralmente são abreviados para args nas documentações do Python.

PROPAGANDA

Parâmetros ou argumentos?
Os termos parâmetro e argumento podem ser usados ​​para a mesma coisa: informações que são passadas para uma função.

Do ponto de vista de uma função:

Um parâmetro é a variável listada entre parênteses na definição da função.

Um argumento é o valor que é enviado para a função quando ela é chamada.

Número de argumentos
Por padrão, uma função deve ser chamada com o número correto de argumentos. Isso significa que, se sua função espera 2 argumentos, você deve chamar a função com 2 argumentos, nem mais, nem menos.

Exemplo
Esta função espera 2 argumentos e obtém 2 argumentos:

def my_function(fname, lname):
  print(fname + " " + lname)

my_function("Emil", "Refsnes")
Se você tentar chamar a função com 1 ou 3 argumentos, receberá um erro:
Exemplo
Esta função espera 2 argumentos, mas obtém apenas 1:

def my_function(fname, lname):
  print(fname + " " + lname)

my_function("Emil")
Argumentos arbitrários, *args
Se você não souber quantos argumentos serão passados ​​para sua função, adicione um *antes do nome do parâmetro na definição da função.

Dessa forma, a função receberá uma tupla de argumentos e poderá acessar os itens de acordo:

Exemplo
Se o número de argumentos for desconhecido, adicione um *antes do nome do parâmetro:

def my_function(*kids):
  print("The youngest child is " + kids[2])

my_function("Emil", "Tobias", "Linus")
Argumentos arbitrários são frequentemente abreviados para *args nas documentações do Python.

Argumentos de palavra-chave
Você também pode enviar argumentos com a sintaxe key = value .

Desta forma, a ordem dos argumentos não importa.

Exemplo
def my_function(child3, child2, child1):
  print("The youngest child is " + child3)

my_function(child1 = "Emil", child2 = "Tobias", child3 = "Linus")
A frase Argumentos de palavras -chave geralmente é abreviada para kwargs nas documentações do Python.

Argumentos arbitrários de palavras-chave, **kwargs
Se você não souber quantos argumentos de palavra-chave serão passados ​​para sua função, adicione dois asteriscos: **antes do nome do parâmetro na definição da função.

Desta forma a função receberá um dicionário de argumentos, podendo acessar os itens de acordo:

Exemplo
Se o número de argumentos de palavra-chave for desconhecido, adicione um duplo **antes do nome do parâmetro:

def my_function(**kid):
  print("His last name is " + kid["lname"])

my_function(fname = "Tobias", lname = "Refsnes")
Argumentos Kword arbitrários são frequentemente abreviados para **kwargs nas documentações do Python.

Valor do parâmetro padrão
O exemplo a seguir mostra como usar um valor de parâmetro padrão.

Se chamarmos a função sem argumento, ela usará o valor padrão:

Exemplo
def my_function(country = "Norway"):
  print("I am from " + country)

my_function("Sweden")
my_function("India")
my_function()
my_function("Brazil")
Passando uma lista como um argumento
Você pode enviar qualquer tipo de dado de argumento para uma função (string, número, lista, dicionário etc.), e ele será tratado como o mesmo tipo de dado dentro da função.

Por exemplo, se você enviar uma lista como argumento, ela ainda será uma lista quando chegar à função:

Exemplo
def my_function(food):
  for x in food:
    print(x)

fruits = ["apple", "banana", "cherry"]

my_function(fruits)
Valores de retorno
Para permitir que uma função retorne um valor, use a return instrução:

Exemplo
def my_function(x):
  return 5 * x

print(my_function(3))
print(my_function(5))
print(my_function(9))
A declaração de passagem
functionAs definições não podem estar vazias, mas se por algum motivo você tiver uma functiondefinição sem conteúdo, coloque a passdeclaração para evitar erros.

Exemplo
def myfunction():
  pass
Recursão
Python também aceita recursão de função, o que significa que uma função definida pode chamar a si mesma.

A recursão é um conceito matemático e de programação comum. Isso significa que uma função chama a si mesma. Isso tem a vantagem de significar que você pode percorrer os dados para chegar a um resultado.

O desenvolvedor deve ter muito cuidado com a recursão, pois pode ser muito fácil escrever uma função que nunca termina, ou uma que usa quantidades excessivas de memória ou poder do processador. No entanto, quando escrita corretamente, a recursão pode ser uma abordagem de programação muito eficiente e matematicamente elegante.

Neste exemplo, tri_recursion() é uma função que definimos para chamar a si mesma ("recurse"). Usamos a variável k como os dados, que decrementam ( -1 ) toda vez que recorremos. A recursão termina quando a condição não for maior que 0 (ou seja, quando for 0).

Para um novo desenvolvedor, pode levar algum tempo para descobrir exatamente como isso funciona, a melhor maneira de descobrir é testando e modificando.

Exemplo
Exemplo de recursão

def tri_recursion(k):
  if(k > 0):
    result = k + tri_recursion(k - 1)
    print(result)
  else:
    result = 0
  return result

print("\n\nRecursion Example Results")
tri_recursion(6)
