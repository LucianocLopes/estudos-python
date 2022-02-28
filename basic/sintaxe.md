Sintaxe do Python
Executar sintaxe do Python
Como aprendemos na página anterior, a sintaxe do Python pode ser executada escrevendo diretamente na linha de comando:

>>> print("Hello, World!")
Hello, World!

Ou criando um arquivo python no servidor, usando a extensão de arquivo .py e executando-o na linha de comando:

C:\Users\Your Name>python myfile.py
Recuo Python
O recuo refere-se aos espaços no início de uma linha de código.

Onde em outras linguagens de programação o recuo no código é apenas para legibilidade, o recuo em Python é muito importante.

Python usa recuo para indicar um bloco de código.

Exemplo
if 5 > 2:
  print("Five is greater than two!")
Python lhe dará um erro se você pular o recuo:

Exemplo
Erro de sintaxe:

if 5 > 2:
print("Five is greater than two!")
O número de espaços depende de você como programador, mas tem que ser pelo menos um.

Exemplo
if 5 > 2:
 print("Five is greater than two!") 
if 5 > 2:
        print("Five is greater than two!") 
Você precisa usar o mesmo número de espaços no mesmo bloco de código, caso contrário, o Python fornecerá um erro:

Exemplo
Erro de sintaxe:

if 5 > 2:
 print("Five is greater than two!")
        print("Five is greater than two!")

Variáveis ​​Python
Em Python, as variáveis ​​são criadas quando você atribui um valor a ela:

Exemplo
Variáveis ​​em Python:

x = 5
y = "Hello, World!"
Python não tem comando para declarar uma variável.

Você aprenderá mais sobre variáveis ​​no capítulo Variáveis ​​do Python .

Comentários
O Python tem capacidade de comentários para fins de documentação no código.

Os comentários começam com um # e o Python renderizará o restante da linha como um comentário:

Exemplo
Comentários em Python:

#This is a comment.
print("Hello, World!")
