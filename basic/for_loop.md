Python para loops
Python para loops
Um loop for é usado para iterar sobre uma sequência (que é uma lista, uma tupla, um dicionário, um conjunto ou uma string).

Isso é menos parecido com a palavra-chave for em outras linguagens de programação e funciona mais como um método iterador, conforme encontrado em outras linguagens de programação orientadas a objetos.

Com o loop for podemos executar um conjunto de instruções, uma vez para cada item de uma lista, tupla, conjunto etc.

Exemplo
Imprima cada fruta em uma lista de frutas:

fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
O loop for não requer que uma variável de indexação seja definida antecipadamente.

Fazendo um loop em uma string
Mesmo as strings são objetos iteráveis, elas contêm uma sequência de caracteres:

Exemplo
Percorra as letras da palavra "banana":

for x in "banana":
  print(x)
A declaração de pausa
Com a instrução break podemos parar o loop antes que ele tenha percorrido todos os itens:

Exemplo
Saia do loop quando xfor "banana":

fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
  if x == "banana":
    break
Exemplo
Saia do loop quando xfor "banana", mas dessa vez o break vem antes do print:

fruits = ["apple", "banana", "cherry"]
for x in fruits:
  if x == "banana":
    break
  print(x)
PROPAGANDA

A declaração continua
Com a instrução continue podemos parar a iteração atual do loop e continuar com a próxima:

Exemplo
Não imprima banana:

fruits = ["apple", "banana", "cherry"]
for x in fruits:
  if x == "banana":
    continue
  print(x)
A função intervalo()
Para percorrer um conjunto de código um determinado número de vezes, podemos usar a função range() ,
A função range() retorna uma sequência de números, começando em 0 por padrão e incrementa em 1 (por padrão) e termina em um número especificado.

Exemplo
Usando a função range():

for x in range(6):
  print(x)
Observe que range(6) não são os valores de 0 a 6, mas os valores de 0 a 5.

A função range() tem como padrão 0 como valor inicial, porém é possível especificar o valor inicial adicionando um parâmetro: range(2, 6) , que significa valores de 2 a 6 (mas não incluindo 6):

Exemplo
Usando o parâmetro inicial:

for x in range(2, 6):
  print(x)
A função range() padroniza para incrementar a sequência em 1, porém é possível especificar o valor do incremento adicionando um terceiro parâmetro: range(2, 30, 3 ) :

Exemplo
Incremente a sequência com 3 (o padrão é 1):

for x in range(2, 30, 3):
  print(x)
Mais em For Loop
A elsepalavra-chave em um forloop especifica um bloco de código a ser executado quando o loop for concluído:

Exemplo
Imprima todos os números de 0 a 5 e imprima uma mensagem quando o loop terminar:

for x in range(6):
  print(x)
else:
  print("Finally finished!")
Nota: O elsebloco NÃO será executado se o loop for interrompido por uma breakinstrução.

Exemplo
Quebre o loop quando xfor 3 e veja o que acontece com o elsebloco:

for x in range(6):
  if x == 3: break
  print(x)
else:
  print("Finally finished!")
Loops aninhados
Um loop aninhado é um loop dentro de um loop.

O "loop interno" será executado uma vez para cada iteração do "loop externo":

Exemplo
Imprima cada adjetivo para cada fruta:

adj = ["red", "big", "tasty"]
fruits = ["apple", "banana", "cherry"]

for x in adj:
  for y in fruits:
    print(x, y)
A declaração de passagem
forloops não podem estar vazios, mas se por algum motivo você tiver um forloop sem conteúdo, coloque a passinstrução para evitar erros.

Exemplo
for x in [0, 1, 2]:
  pass

