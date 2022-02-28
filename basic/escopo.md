Escopo do Python
Uma variável só está disponível dentro da região em que foi criada. Isso é chamado de escopo .

Escopo Local
Uma variável criada dentro de uma função pertence ao escopo local dessa função e só pode ser usada dentro dessa função.

Exemplo
Uma variável criada dentro de uma função está disponível dentro dessa função:

def myfunc():
  x = 300
  print(x)

myfunc()
Função Dentro da Função
Conforme explicado no exemplo acima, a variável xnão está disponível fora da função, mas está disponível para qualquer função dentro da função:

Exemplo
A variável local pode ser acessada de uma função dentro da função:

def myfunc():
  x = 300
  def myinnerfunc():
    print(x)
  myinnerfunc()

myfunc()
PROPAGANDA

Âmbito global
Uma variável criada no corpo principal do código Python é uma variável global e pertence ao escopo global.

As variáveis ​​globais estão disponíveis em qualquer escopo, global e local.

Exemplo
Uma variável criada fora de uma função é global e pode ser usada por qualquer pessoa:

x = 300

def myfunc():
  print(x)

myfunc()

print(x)
Variáveis ​​de nomenclatura
Se você operar com o mesmo nome de variável dentro e fora de uma função, o Python as tratará como duas variáveis ​​separadas, uma disponível no escopo global (fora da função) e outra disponível no escopo local (dentro da função):

Exemplo
A função imprimirá o local xe, em seguida, o código imprimirá o global x:

x = 300

def myfunc():
  x = 200
  print(x)

myfunc()

print(x)
Palavra-chave global
Se você precisar criar uma variável global, mas estiver preso no escopo local, poderá usar a palavra- globalchave.

A palavra- globalchave torna a variável global.

Exemplo
Se você usar a palavra- globalchave, a variável pertence ao escopo global:

def myfunc():
  global x
  x = 300

myfunc()

print(x)
Além disso, use a palavra- globalchave se quiser fazer uma alteração em uma variável global dentro de uma função.

Exemplo
Para alterar o valor de uma variável global dentro de uma função, consulte a variável usando a globalpalavra-chave:

x = 300

def myfunc():
  global x
  x = 200

myfunc()

print(x)