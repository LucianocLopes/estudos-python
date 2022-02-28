Números Python
Números Python
Existem três tipos numéricos em Python:

int
float
complex
Variáveis ​​de tipos numéricos são criadas quando você atribui um valor a elas:

Exemplo
x = 1    # int
y = 2.8  # float
z = 1j   # complex
Para verificar o tipo de qualquer objeto em Python, use a type()função:

Exemplo
print(type(x))
print(type(y))
print(type(z))
Int
Int, ou inteiro, é um número inteiro, positivo ou negativo, sem decimais, de comprimento ilimitado.

Exemplo
Inteiros:

x = 1
y = 35656222554887711
z = -3255522

print(type(x))
print(type(y))
print(type(z))
Flutuador
Float, ou "número de ponto flutuante" é um número, positivo ou negativo, contendo um ou mais decimais.

Exemplo
Flutuadores:

x = 1.10
y = 1.0
z = -35.59

print(type(x))
print(type(y))
print(type(z))
Float também pode ser números científicos com um "e" para indicar a potência de 10.

Exemplo
Flutuadores:

x = 35e3
y = 12E4
z = -87.7e100

print(type(x))
print(type(y))
print(type(z))

Complexo
Os números complexos são escritos com um "j" como a parte imaginária:

Exemplo
Complexo:

x = 3+5j
y = 5j
z = -5j

print(type(x))
print(type(y))
print(type(z))
Conversão de tipo
Você pode converter de um tipo para outro com os métodos int(), float()e :complex()

Exemplo
Converter de um tipo para outro:

x = 1    # int
y = 2.8  # float
z = 1j   # complex

#convert from int to float:
a = float(x)

#convert from float to int:
b = int(y)

#convert from int to complex:
c = complex(x)

print(a)
print(b)
print(c)

print(type(a))
print(type(b))
print(type(c))
Nota: Você não pode converter números complexos em outro tipo de número.

Número aleatório
Python não tem uma random()função para fazer um número aleatório, mas Python tem um módulo embutido chamado randomque pode ser usado para fazer números aleatórios:

Exemplo
Importe o módulo aleatório e exiba um número aleatório entre 1 e 9:

import random

print(random.randrange(1, 10))
Em nosso Random Module Reference você aprenderá mais sobre o módulo Random.

