# Booleanos Python

Booleanos representam um dos dois valores: `True` ou `False`.

**Valores Booleanos**
Na programação, muitas vezes você precisa saber se uma expressão é True ou False.
Você pode avaliar qualquer expressão em Python e obter uma das duas respostas, True ou False.
Quando você compara dois valores, a expressão é avaliada e o Python retorna a resposta booleana:
Exemplo

```py
print(10 > 9)
print(10 == 9)
print(10 < 9)
```

Quando você executa uma condição em uma instrução `if`, o Python retorna True ou False:
Exemplo
Imprima uma mensagem com base em se a condição é True ou False:

```py
a = 200
b = 33

if b > a:
  print("b is greater than a")
else:
  print("b is not greater than a")
```

Avaliar Valores e Variáveis
A função bool() permite avaliar qualquer valor e dar a você True ou False em troca.
Exemplo
Avalie uma string e um número:

```py
print(bool("Hello"))
print(bool(15))
```

Exemplo
Avalie duas variáveis:

```py
x = "Hello"
y = 15

print(bool(x))
print(bool(y))
```

**A maioria dos valores são verdadeiros**
Quase todos valores são avaliados como True se tiver algum tipo de conteúdo.
  - Qualquer string é True, exceto strings vazias.
  - Qualquer número é True, exceto 0.
  - Qualquer lista, tupla, conjunto e dicionário são True, exceto os vazios.

Exemplo
O seguinte retornará True:
```py
bool("abc")
bool(123)
bool(["apple", "cherry", "banana"])
```

**Valores são falsos**
Na verdade, não há muitos valores avaliados para False, exceto valores vazios, como `()`, `[]`, `{}`, `""`, o número `0` e o valor `None`. E, claro, o valor é False avaliado como False.
Exemplo
O seguinte retornará False:

```py
bool(False)
bool(None)
bool(0)
bool("")
bool(())
bool([])
bool({})
```

Mais um valor, ou objeto neste caso, é avaliado como False, e isso é se você tem um objeto que é feito de uma classe com uma função `__len__` que retorna `0` ou False:
Exemplo

```py
class myclass():
  def __len__(self):
    return 0

myobj = myclass()
print(bool(myobj))
```

**Funções podem retornar um booleano**
Você pode criar funções que retornam um valor booleano:
Exemplo
Imprima a resposta de uma função:

```py
def myFunction() :
  return True

print(myFunction())
```

Você pode executar o código com base na resposta booleana de uma função:
Exemplo
Imprima "SIM!" se a função retornar True, caso contrário imprima "NÃO!":

```py
def myFunction() :
  return True

if myFunction():
  print("YES!")
else:
  print("NO!")
```

O Python também possui muitas funções internas que retornam um valor booleano, como a função isinstance(), que pode ser usada para determinar se um objeto é de um determinado tipo de dados:
Exemplo
Verifique se um objeto é um inteiro ou não:

```py
x = 200
print(isinstance(x, int))
```
