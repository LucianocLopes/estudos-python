Python Se... Senão
Condições do Python e instruções If
Python suporta as condições lógicas usuais da matemática:

Igual a: a == b
Diferentes: a != b
Menor que: a < b
Menor ou igual a: a <= b
Maior que: a > b
Maior ou igual a: a >= b
Essas condições podem ser usadas de várias maneiras, mais comumente em "instruções if" e loops.

Uma "instrução if" é escrita usando a palavra-chave if .

Exemplo
Se declaração:

a = 33
b = 200
if b > a:
  print("b is greater than a")
Neste exemplo, usamos duas variáveis, a e b , que são usadas como parte da instrução if para testar se b é maior que a . Como a é 33 , e b é 200 , sabemos que 200 é maior que 33, e então imprimimos na tela que "b é maior que a".

Recuo
Python conta com recuo (espaço em branco no início de uma linha) para definir o escopo no código. Outras linguagens de programação costumam usar colchetes para essa finalidade.

Exemplo
Se declaração, sem recuo (irá gerar um erro):

a = 33
b = 200
if b > a:
print("b is greater than a") # you will get an error
PROPAGANDA

Elif
A palavra-chave elif é uma maneira pythons de dizer "se as condições anteriores não forem verdadeiras, tente esta condição".

Exemplo
a = 33
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
Neste exemplo a é igual a b , então a primeira condição não é verdadeira, mas a condição elif é verdadeira, então imprimimos na tela que "a e b são iguais".

Outro
A palavra-chave else captura qualquer coisa que não seja capturada pelas condições anteriores.

Exemplo
a = 200
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
else:
  print("a is greater than b")
Neste exemplo a é maior que b , então a primeira condição não é verdadeira, também a condição elif não é verdadeira, então vamos para a condição else e imprimimos na tela que "a é maior que b".

Você também pode ter um elsesem o elif:

Exemplo
a = 200
b = 33
if b > a:
  print("b is greater than a")
else:
  print("b is not greater than a")
Mão curta se
Se você tiver apenas uma instrução para executar, poderá colocá-la na mesma linha da instrução if.

Exemplo
Uma linha if declaração:

if a > b: print("a is greater than b")
Mão curta Se... Senão
Se você tiver apenas uma instrução para executar, uma para if e outra para else, você pode colocar tudo na mesma linha:

Exemplo
Uma linha if else instrução:

a = 2
b = 330
print("A") if a > b else print("B")
Essa técnica é conhecida como Operadores Ternários ou Expressões Condicionais .

Você também pode ter várias instruções else na mesma linha:

Exemplo
Uma linha if else instrução, com 3 condições:

a = 330
b = 330
print("A") if a > b else print("=") if a == b else print("B")
E
A palavra-chave and é um operador lógico e é usada para combinar instruções condicionais:

Exemplo
Teste se afor maior que b, E se c for maior que a:

a = 200
b = 33
c = 500
if a > b and c > a:
  print("Both conditions are True")
Ou
A orpalavra-chave é um operador lógico e é usada para combinar instruções condicionais:

Exemplo
Teste se afor maior que b, OU se a for maior que c:

a = 200
b = 33
c = 500
if a > b or a > c:
  print("At least one of the conditions is True")
Se aninhado
Você pode ter ifinstruções dentro ifde instruções, isso é chamado de instruções aninhadas if .

Exemplo
x = 41

if x > 10:
  print("Above ten,")
  if x > 20:
    print("and also above 20!")
  else:
    print("but not above 20.")
A declaração de passagem
ifdeclarações não podem ser vazias, mas se você por algum motivo tiver uma ifdeclaração sem conteúdo, coloque a passdeclaração para evitar erros.

Exemplo
a = 33
b = 200

if b > a:
  pass

