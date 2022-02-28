Python Lambda
Uma função lambda é uma pequena função anônima.

Uma função lambda pode receber qualquer número de argumentos, mas pode ter apenas uma expressão.

Sintaxe
lambda arguments : expression
A expressão é executada e o resultado é retornado:

Exemplo
Adicione 10 ao argumento ae retorne o resultado:

x = lambda a : a + 10
print(x(5))
As funções lambda podem receber qualquer número de argumentos:

Exemplo
Multiplique argumento apor argumento be retorne o resultado:

x = lambda a, b : a * b
print(x(5, 6))
Exemplo
Resuma argument a, b, and ce retorne o resultado:

x = lambda a, b, c : a + b + c
print(x(5, 6, 2))
PROPAGANDA

Por que usar funções do Lambda?
O poder do lambda é melhor mostrado quando você os usa como uma função anônima dentro de outra função.

Digamos que você tenha uma definição de função que recebe um argumento e esse argumento será multiplicado por um número desconhecido:

def myfunc(n):
  return lambda a : a * n
Use essa definição de função para fazer uma função que sempre duplique o número que você envia:

Exemplo
def myfunc(n):
  return lambda a : a * n

mydoubler = myfunc(2)

print(mydoubler(11))
Ou use a mesma definição de função para fazer uma função que sempre triplique o número que você envia:

Exemplo
def myfunc(n):
  return lambda a : a * n

mytripler = myfunc(3)

print(mytripler(11))
Ou use a mesma definição de função para fazer as duas funções, no mesmo programa:

Exemplo
def myfunc(n):
  return lambda a : a * n

mydoubler = myfunc(2)
mytripler = myfunc(3)

print(mydoubler(11))
print(mytripler(11))
Use funções lambda quando uma função anônima for necessária por um curto período de tempo.