Python JSON
JSON é uma sintaxe para armazenar e trocar dados.

JSON é texto, escrito com notação de objeto JavaScript.

JSON em Python
Python tem um pacote embutido chamado json, que pode ser usado para trabalhar com dados JSON.

Exemplo
Importe o módulo json:

import json
Parse JSON - Converter de JSON para Python
Se você tiver uma string JSON, poderá analisá-la usando o json.loads()método.

O resultado será um dicionário Python .

Exemplo
Converter de JSON para Python:

import json

# some JSON:
x =  '{ "name":"John", "age":30, "city":"New York"}'

# parse x:
y = json.loads(x)

# the result is a Python dictionary:
print(y["age"])
Converter de Python para JSON
Se você tiver um objeto Python, poderá convertê-lo em uma string JSON usando o json.dumps()método.

Exemplo
Converter de Python para JSON:

import json

# a Python object (dict):
x = {
  "name": "John",
  "age": 30,
  "city": "New York"
}

# convert into JSON:
y = json.dumps(x)

# the result is a JSON string:
print(y)
PROPAGANDA

Você pode converter objetos Python dos seguintes tipos em strings JSON:

ditar
Lista
tupla
corda
int
flutuador
Verdadeiro
Falso
Nenhum
Exemplo
Converta objetos Python em strings JSON e imprima os valores:

import json

print(json.dumps({"name": "John", "age": 30}))
print(json.dumps(["apple", "bananas"]))
print(json.dumps(("apple", "bananas")))
print(json.dumps("hello"))
print(json.dumps(42))
print(json.dumps(31.76))
print(json.dumps(True))
print(json.dumps(False))
print(json.dumps(None))
Quando você converte de Python para JSON, os objetos Python são convertidos no equivalente JSON (JavaScript):

Python	JSON
dict	Object
list	Array
tuple	Array
str	String
int	Number
float	Number
True	true
False	false
None	null
Exemplo
Converta um objeto Python contendo todos os tipos de dados legais:

import json

x = {
  "name": "John",
  "age": 30,
  "married": True,
  "divorced": False,
  "children": ("Ann","Billy"),
  "pets": None,
  "cars": [
    {"model": "BMW 230", "mpg": 27.5},
    {"model": "Ford Edge", "mpg": 24.1}
  ]
}

print(json.dumps(x))
Formate o resultado
O exemplo acima imprime uma string JSON, mas não é muito fácil de ler, sem recuos e quebras de linha.

O json.dumps()método possui parâmetros para facilitar a leitura do resultado:

Exemplo
Use o indentparâmetro para definir os números de recuos:

json.dumps(x, indent=4)
Você também pode definir os separadores, o valor padrão é ("", ", ": "), o que significa usar uma vírgula e um espaço para separar cada objeto e dois pontos e um espaço para separar as chaves dos valores:

Exemplo
Use o separatorsparâmetro para alterar o separador padrão:

json.dumps(x, indent=4, separators=(". ", " = "))
Encomende o resultado
O json.dumps()método possui parâmetros para ordenar as chaves no resultado:

Exemplo
Use o sort_keysparâmetro para especificar se o resultado deve ser classificado ou não:

json.dumps(x, indent=4, sort_keys=True)