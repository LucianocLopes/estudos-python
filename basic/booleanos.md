Booleanos Python
Booleanos representam um dos dois valores: Trueou False.

Valores Booleanos
Na programação, muitas vezes você precisa saber se uma expressão é Trueou False.

Você pode avaliar qualquer expressão em Python e obter uma das duas respostas, Trueou False.

Quando você compara dois valores, a expressão é avaliada e o Python retorna a resposta booleana:

Exemplo
print(10 > 9)
print(10 == 9)
print(10 < 9)
Quando você executa uma condição em uma instrução if, o Python retorna Trueou False:

Exemplo
Imprima uma mensagem com base em se a condição é Trueou False:

a = 200
b = 33

if b > a:
  print("b is greater than a")
else:
  print("b is not greater than a")
Avaliar Valores e Variáveis
A bool()função permite avaliar qualquer valor e dar a você Trueou False em troca,

Exemplo
Avalie uma string e um número:

print(bool("Hello"))
print(bool(15))
Exemplo
Avalie duas variáveis:

x = "Hello"
y = 15

print(bool(x))
print(bool(y))
PROPAGANDA

A maioria dos valores são verdadeiros
Quase qualquer valor é avaliado Truese tiver algum tipo de conteúdo.

Qualquer string é True, exceto strings vazias.

Qualquer número é True, exceto 0.

Qualquer lista, tupla, conjunto e dicionário são True, exceto os vazios.

Exemplo
O seguinte retornará True:

bool("abc")
bool(123)
bool(["apple", "cherry", "banana"])
Alguns valores são falsos
Na verdade, não há muitos valores avaliados para False, exceto valores vazios, como (), [], {}, "", o número 0e o valor None. E, claro, o valor é Falseavaliado como False.

Exemplo
O seguinte retornará False:

bool(False)
bool(None)
bool(0)
bool("")
bool(())
bool([])
bool({})
Mais um valor, ou objeto neste caso, é avaliado como False, e isso é se você tem um objeto que é feito de uma classe com uma __len__função que retorna 0ou False:

Exemplo
class myclass():
  def __len__(self):
    return 0

myobj = myclass()
print(bool(myobj))
Funções podem retornar um booleano
Você pode criar funções que retornam um valor booleano:

Exemplo
Imprima a resposta de uma função:

def myFunction() :
  return True

print(myFunction())
Você pode executar o código com base na resposta booleana de uma função:

Exemplo
Imprima "SIM!" se a função retornar True, caso contrário imprima "NO!":

def myFunction() :
  return True

if myFunction():
  print("YES!")
else:
  print("NO!")
O Python também possui muitas funções internas que retornam um valor booleano, como a isinstance() função, que pode ser usada para determinar se um objeto é de um determinado tipo de dados:

Exemplo
Verifique se um objeto é um inteiro ou não:

x = 200
print(isinstance(x, int))
