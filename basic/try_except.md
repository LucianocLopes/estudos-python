Python Tente Exceto
O trybloco permite testar um bloco de código quanto a erros.

O exceptbloco permite que você lide com o erro.

O elsebloco permite executar código quando não há erro.

O finallybloco permite que você execute código, independentemente do resultado dos blocos try e except.

Manipulação de exceção
Quando ocorre um erro, ou exceção, como chamamos, o Python normalmente para e gera uma mensagem de erro.

Essas exceções podem ser tratadas usando a tryinstrução:

Exemplo
O trybloco irá gerar uma exceção, pois xnão está definido:

try:
  print(x)
except:
  print("An exception occurred")
Como o bloco try gera um erro, o bloco except será executado.

Sem o bloco try, o programa irá travar e gerar um erro:

Exemplo
Esta declaração irá gerar um erro, porque xnão está definido:

print(x)
Muitas exceções
Você pode definir quantos blocos de exceção desejar, por exemplo, se você deseja executar um bloco de código especial para um tipo especial de erro:

Exemplo
Imprima uma mensagem se o bloco try gerar a NameErrore outra para outros erros:

try:
  print(x)
except NameError:
  print("Variable x is not defined")
except:
  print("Something else went wrong")
PROPAGANDA

Outro
Você pode usar a elsepalavra-chave para definir um bloco de código a ser executado se nenhum erro for gerado:

Exemplo
Neste exemplo, o trybloco não gera nenhum erro:

try:
  print("Hello")
except:
  print("Something went wrong")
else:
  print("Nothing went wrong")
Finalmente
O finallybloco, se especificado, será executado independentemente de o bloco try gerar um erro ou não.

Exemplo
try:
  print(x)
except:
  print("Something went wrong")
finally:
  print("The 'try except' is finished")
Isso pode ser útil para fechar objetos e limpar recursos:

Exemplo
Tente abrir e gravar em um arquivo que não seja gravável:

try:
  f = open("demofile.txt")
  try:
    f.write("Lorum Ipsum")
  except:
    print("Something went wrong when writing to the file")
  finally:
    f.close()
except:
  print("Something went wrong when opening the file")
O programa pode continuar, sem deixar o objeto de arquivo aberto.

Criar uma exceção
Como desenvolvedor Python, você pode optar por lançar uma exceção se ocorrer uma condição.

Para lançar (ou levantar) uma exceção, use a palavra- raisechave.

Exemplo
Gere um erro e pare o programa se x for menor que 0:

x = -1

if x < 0:
  raise Exception("Sorry, no numbers below zero")
A raisepalavra-chave é usada para gerar uma exceção.

Você pode definir que tipo de erro gerar e o texto a ser impresso para o usuário.

Exemplo
Gere um TypeError se x não for um inteiro:

x = "hello"

if not type(x) is int:
  raise TypeError("Only integers are allowed")