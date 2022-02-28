Strings Python
Cordas
Strings em python são cercadas por aspas simples ou aspas duplas.

'olá' é o mesmo que "olá" .

Você pode exibir um literal de string com a print()função:

Exemplo
print("Hello")
print('Hello')
Atribuir String a uma Variável
A atribuição de uma string a uma variável é feita com o nome da variável seguido por um sinal de igual e a string:

Exemplo
a = "Hello"
print(a)
Strings de várias linhas
Você pode atribuir uma string de várias linhas a uma variável usando três aspas:

Exemplo
Você pode usar três aspas duplas:

a = """Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua."""
print(a)
Ou três aspas simples:

Exemplo
a = '''Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua.'''
print(a)
Nota: no resultado, as quebras de linha são inseridas na mesma posição do código.

PROPAGANDA

Strings são Arrays
Como muitas outras linguagens de programação populares, strings em Python são arrays de bytes que representam caracteres unicode.

No entanto, o Python não possui um tipo de dados de caractere, um único caractere é simplesmente uma string com um comprimento de 1.

Colchetes podem ser usados ​​para acessar elementos da string.

Exemplo
Pegue o caractere na posição 1 (lembre-se que o primeiro caractere tem a posição 0):

a = "Hello, World!"
print(a[1])
Fazendo um loop em uma string
Como strings são arrays, podemos fazer um loop pelos caracteres em uma string, com um forloop.

Exemplo
Percorra as letras da palavra "banana":

for x in "banana":
  print(x)
Saiba mais sobre For Loops em nosso capítulo Python For Loops .

Comprimento da string
Para obter o comprimento de uma string, use a len()função.

Exemplo
A len()função retorna o comprimento de uma string:

a = "Hello, World!"
print(len(a))
String de verificação
Para verificar se uma determinada frase ou caractere está presente em uma string, podemos usar a palavra-chave in.

Exemplo
Verifique se "grátis" está presente no texto a seguir:

txt = "The best things in life are free!"
print("free" in txt)
Use-o em uma ifdeclaração:

Exemplo
Imprima apenas se "grátis" estiver presente:

txt = "The best things in life are free!"
if "free" in txt:
  print("Yes, 'free' is present.")
Aprenda mais sobre instruções If em nosso capítulo If...Else do Python .

Verifique se NÃO
Para verificar se uma determinada frase ou caractere NÃO está presente em uma string, podemos usar a palavra-chave not in.

Exemplo
Verifique se "caro" NÃO está presente no texto a seguir:

txt = "The best things in life are free!"
print("expensive" not in txt)
Use-o em uma ifdeclaração:

Exemplo
imprima somente se "caro" NÃO estiver presente:

txt = "The best things in life are free!"
if "expensive" not in txt:
  print("No, 'expensive' is NOT present.")

Python - Fatiando Strings
Fatiamento
Você pode retornar um intervalo de caracteres usando a sintaxe de fatia.

Especifique o índice inicial e o índice final, separados por dois pontos, para retornar uma parte da string.

Exemplo
Obtenha os personagens da posição 2 para a posição 5 (não incluído):

b = "Hello, World!"
print(b[2:5])
Nota: O primeiro caractere tem índice 0.

Fatia desde o início
Ao deixar de fora o índice inicial, o intervalo começará no primeiro caractere:

Exemplo
Obtenha os personagens desde o início até a posição 5 (não incluído):

b = "Hello, World!"
print(b[:5])
PROPAGANDA

Fatie até o fim
Ao deixar de fora o índice final , o intervalo irá para o final:

Exemplo
Pegue os personagens da posição 2 e até o final:

b = "Hello, World!"
print(b[2:])
Indexação negativa
Use índices negativos para iniciar a fatia a partir do final da string:
Exemplo
Obtenha os personagens:

De: "o" em "Mundo!" (posição -5)

Para, mas não incluído: "d" em "Mundo!" (posição -2):

b = "Hello, World!"
print(b[-5:-2])

Python - Modificar Strings
Python tem um conjunto de métodos integrados que você pode usar em strings.

Maiúsculas
Exemplo
O upper()método retorna a string em maiúsculas:

a = "Hello, World!"
print(a.upper())
Minúsculas
Exemplo
O lower()método retorna a string em letras minúsculas:

a = "Hello, World!"
print(a.lower())
Remover espaço em branco
Espaço em branco é o espaço antes e/ou depois do texto real e, muitas vezes, você deseja remover esse espaço.

Exemplo
O strip()método remove qualquer espaço em branco do início ou do fim:

a = " Hello, World! "
print(a.strip()) # returns "Hello, World!"
PROPAGANDA

Substituir Cadeia
Exemplo
O replace()método substitui uma string por outra string:

a = "Hello, World!"
print(a.replace("H", "J"))
Sequência dividida
O split()método retorna uma lista onde o texto entre o separador especificado se torna os itens da lista.

Exemplo
O split()método divide a string em substrings se encontrar instâncias do separador:

a = "Hello, World!"
print(a.split(",")) # returns ['Hello', ' World!']
Saiba mais sobre Listas em nosso capítulo Listas do Python .

Métodos de string
Saiba mais sobre Métodos de String com nossa Referência de Métodos de String

Python - Concatenação de Strings
Concatenação de String
Para concatenar ou combinar duas strings você pode usar o operador +.

Exemplo
Mesclar variável acom variável bem variável c:

a = "Hello"
b = "World"
c = a + b
print(c)
Exemplo
Para adicionar um espaço entre eles, adicione um " ":

a = "Hello"
b = "World"
c = a + " " + b
print(c)

Python - Formato - Strings
Formato de string
Como aprendemos no capítulo Variáveis ​​do Python, não podemos combinar strings e números assim:

Exemplo
age = 36
txt = "My name is John, I am " + age
print(txt)
Mas podemos combinar strings e números usando o format()método!

O format()método pega os argumentos passados, os formata e os coloca na string onde {}estão os espaços reservados:

Exemplo
Use o format()método para inserir números em strings:

age = 36
txt = "My name is John, and I am {}"
print(txt.format(age))
O método format() recebe um número ilimitado de argumentos e são colocados nos respectivos espaços reservados:

Exemplo
quantity = 3
itemno = 567
price = 49.95
myorder = "I want {} pieces of item {} for {} dollars."
print(myorder.format(quantity, itemno, price))
Você pode usar números de índice {0}para garantir que os argumentos sejam colocados nos espaços reservados corretos:

Exemplo
quantity = 3
itemno = 567
price = 49.95
myorder = "I want to pay {2} dollars for {0} pieces of item {1}."
print(myorder.format(quantity, itemno, price))
Saiba mais sobre a formatação de strings em nosso capítulo sobre formatação de strings .

Python - Caracteres de escape
Caractere de Fuga
Para inserir caracteres ilegais em uma string, use um caractere de escape.

Um caractere de escape é uma barra invertida \seguida pelo caractere que você deseja inserir.

Um exemplo de um caractere ilegal é uma aspa dupla dentro de uma string que é cercada por aspas duplas:

Exemplo
Você receberá um erro se usar aspas duplas dentro de uma string cercada por aspas duplas:

txt = "We are the so-called "Vikings" from the north."
Para corrigir esse problema, use o caractere de escape \":

Exemplo
O caractere de escape permite que você use aspas duplas quando normalmente não seria permitido:

txt = "We are the so-called \"Vikings\" from the north."
Caracteres de escape
Outros caracteres de escape usados ​​em Python:

Code	Result	Try it
\'	Single Quote	
\\	Backslash	
\n	New Line	
\r	Carriage Return	
\t	Tab	
\b	Backspace	
\f	Form Feed	
\ooo	Octal value	
\xhh	Hex value

Python - Métodos de String
Métodos de string
Python tem um conjunto de métodos integrados que você pode usar em strings.

Nota: Todos os métodos de string retornam novos valores. Eles não alteram a string original.

Method	Description
capitalize()	Converts the first character to upper case
casefold()	Converts string into lower case
center()	Returns a centered string
count()	Returns the number of times a specified value occurs in a string
encode()	Returns an encoded version of the string
endswith()	Returns true if the string ends with the specified value
expandtabs()	Sets the tab size of the string
find()	Searches the string for a specified value and returns the position of where it was found
format()	Formats specified values in a string
format_map()	Formats specified values in a string
index()	Searches the string for a specified value and returns the position of where it was found
isalnum()	Returns True if all characters in the string are alphanumeric
isalpha()	Returns True if all characters in the string are in the alphabet
isdecimal()	Returns True if all characters in the string are decimals
isdigit()	Returns True if all characters in the string are digits
isidentifier()	Returns True if the string is an identifier
islower()	Returns True if all characters in the string are lower case
isnumeric()	Returns True if all characters in the string are numeric
isprintable()	Returns True if all characters in the string are printable
isspace()	Returns True if all characters in the string are whitespaces
istitle()	Returns True if the string follows the rules of a title
isupper()	Returns True if all characters in the string are upper case
join()	Joins the elements of an iterable to the end of the string
ljust()	Returns a left justified version of the string
lower()	Converts a string into lower case
lstrip()	Returns a left trim version of the string
maketrans()	Returns a translation table to be used in translations
partition()	Returns a tuple where the string is parted into three parts
replace()	Returns a string where a specified value is replaced with a specified value
rfind()	Searches the string for a specified value and returns the last position of where it was found
rindex()	Searches the string for a specified value and returns the last position of where it was found
rjust()	Returns a right justified version of the string
rpartition()	Returns a tuple where the string is parted into three parts
rsplit()	Splits the string at the specified separator, and returns a list
rstrip()	Returns a right trim version of the string
split()	Splits the string at the specified separator, and returns a list
splitlines()	Splits the string at line breaks and returns a list
startswith()	Returns true if the string starts with the specified value
strip()	Returns a trimmed version of the string
swapcase()	Swaps cases, lower case becomes upper case and vice versa
title()	Converts the first character of each word to upper case
translate()	Returns a translated string
upper()	Converts a string into upper case
zfill()	Fills the string with a specified number of 0 values at the beginning

