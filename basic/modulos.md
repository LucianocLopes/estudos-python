Módulos Python
O que é um Módulo?
Considere um módulo como sendo o mesmo que uma biblioteca de código.

Um arquivo contendo um conjunto de funções que você deseja incluir em seu aplicativo.

Criar um módulo
Para criar um módulo basta salvar o código desejado em um arquivo com a extensão de arquivo .py:

Exemplo
Salve este código em um arquivo chamadomymodule.py

def greeting(name):
  print("Hello, " + name)
Usar um módulo
Agora podemos usar o módulo que acabamos de criar, usando a importinstrução:

Exemplo
Importe o módulo chamado mymodule e chame a função de saudação:

import mymodule

mymodule.greeting("Jonathan")
Nota: Ao usar uma função de um módulo, use a sintaxe: module_name.function_name .

Variáveis ​​no Módulo
O módulo pode conter funções, como já descrito, mas também variáveis ​​de todos os tipos (arrays, dicionários, objetos etc):

Exemplo
Salve este código no arquivomymodule.py

person1 = {
  "name": "John",
  "age": 36,
  "country": "Norway"
}
Exemplo
Importe o módulo chamado mymodule e acesse o dicionário person1:

import mymodule

a = mymodule.person1["age"]
print(a)
PROPAGANDA

Nomeando um Módulo
Você pode nomear o arquivo do módulo como quiser, mas deve ter a extensão do arquivo .py

Renomear um módulo
Você pode criar um alias ao importar um módulo, usando a aspalavra-chave:

Exemplo
Crie um alias para mymodulechamado mx:

import mymodule as mx

a = mx.person1["age"]
print(a)
Módulos integrados
Existem vários módulos integrados no Python, que você pode importar sempre que quiser.

Exemplo
Importe e use o platformmódulo:

import platform

x = platform.system()
print(x)
Usando a função dir()
Existe uma função interna para listar todos os nomes de funções (ou nomes de variáveis) em um módulo. A dir()função:

Exemplo
Liste todos os nomes definidos pertencentes ao módulo da plataforma:

import platform

x = dir(platform)
print(x)
Nota: A função dir() pode ser usada em todos os módulos, inclusive aqueles que você mesmo criar.

Importar do módulo
Você pode optar por importar apenas partes de um módulo, usando a palavra- fromchave.

Exemplo
O módulo nomeado mymoduletem uma função e um dicionário:

def greeting(name):
  print("Hello, " + name)

person1 = {
  "name": "John",
  "age": 36,
  "country": "Norway"
}
Exemplo
Importe apenas o dicionário person1 do módulo:

from mymodule import person1

print (person1["age"])
Nota: Ao importar usando a palavra- from chave, não use o nome do módulo ao fazer referência a elementos no módulo. Exemplo: person1["age"], não mymodule.person1["age"]