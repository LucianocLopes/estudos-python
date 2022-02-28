Python RegEx
Um RegEx, ou Expressão Regular, é uma sequência de caracteres que forma um padrão de pesquisa.

RegEx pode ser usado para verificar se uma string contém o padrão de pesquisa especificado.

Módulo RegEx
Python tem um pacote embutido chamado re, que pode ser usado para trabalhar com Expressões Regulares.

Importe o remódulo:

import re
RegEx em Python
Depois de importar o remódulo, você pode começar a usar expressões regulares:

Exemplo
Pesquise a string para ver se ela começa com "The" e termina com "Spain":

import re

txt = "The rain in Spain"
x = re.search("^The.*Spain$", txt)
Funções RegEx
O remódulo oferece um conjunto de funções que nos permite pesquisar uma string por uma correspondência:

Function	Description
findall	Returns a list containing all matches
search	Returns a Match object if there is a match anywhere in the string
split	Returns a list where the string has been split at each match
sub	Replaces one or many matches with a string
PROPAGANDA

Metacaracteres
Metacaracteres são caracteres com um significado especial:

Character	Description	Example	Try it
[]	A set of characters	"[a-m]"	
\	Signals a special sequence (can also be used to escape special characters)	"\d"	
.	Any character (except newline character)	"he..o"	
^	Starts with	"^hello"	
$	Ends with	"planet$"	
*	Zero or more occurrences	"he.*o"	
+	One or more occurrences	"he.+o"	
?	Zero or one occurrences	"he.?o"	
{}	Exactly the specified number of occurrences	"he.{2}o"	
|	Either or	"falls|stays"	
()	Capture and group	 	 
Sequências Especiais
Uma sequência especial é \seguida por um dos caracteres na lista abaixo e tem um significado especial:

Character	Description	Example	Try it
\A	Returns a match if the specified characters are at the beginning of the string	"\AThe"	
\b	Returns a match where the specified characters are at the beginning or at the end of a word
(the "r" in the beginning is making sure that the string is being treated as a "raw string")	r"\bain"
r"ain\b"	
\B	Returns a match where the specified characters are present, but NOT at the beginning (or at the end) of a word
(the "r" in the beginning is making sure that the string is being treated as a "raw string")	r"\Bain"
r"ain\B"	
\d	Returns a match where the string contains digits (numbers from 0-9)	"\d"	
\D	Returns a match where the string DOES NOT contain digits	"\D"	
\s	Returns a match where the string contains a white space character	"\s"	
\S	Returns a match where the string DOES NOT contain a white space character	"\S"	
\w	Returns a match where the string contains any word characters (characters from a to Z, digits from 0-9, and the underscore _ character)	"\w"	
\W	Returns a match where the string DOES NOT contain any word characters	"\W"	
\Z	Returns a match if the specified characters are at the end of the string	"Spain\Z"	
Conjuntos
Um conjunto é um conjunto de caracteres dentro de um par de colchetes []com um significado especial:

Set	Description	Try it
[arn]	Returns a match where one of the specified characters (a, r, or n) are present	
[a-n]	Returns a match for any lower case character, alphabetically between a and n	
[^arn]	Returns a match for any character EXCEPT a, r, and n	
[0123]	Returns a match where any of the specified digits (0, 1, 2, or 3) are present	
[0-9]	Returns a match for any digit between 0 and 9	
[0-5][0-9]	Returns a match for any two-digit numbers from 00 and 59	
[a-zA-Z]	Returns a match for any character alphabetically between a and z, lower case OR upper case	
[+]	In sets, +, *, ., |, (), $,{} has no special meaning, so [+] means: return a match for any + character in the string	
 
A função findall()
A findall()função retorna uma lista contendo todas as correspondências.

Exemplo
Imprima uma lista de todas as correspondências:

import re

txt = "The rain in Spain"
x = re.findall("ai", txt)
print(x)
A lista contém as correspondências na ordem em que são encontradas.

Se nenhuma correspondência for encontrada, uma lista vazia será retornada:

Exemplo
Retorna uma lista vazia se nenhuma correspondência foi encontrada:

import re

txt = "The rain in Spain"
x = re.findall("Portugal", txt)
print(x)
 
A função pesquisar()
A search()função procura uma correspondência na string e retorna um objeto Match se houver uma correspondência.

Se houver mais de uma correspondência, apenas a primeira ocorrência da correspondência será retornada:

Exemplo
Procure o primeiro caractere de espaço em branco na string:

import re

txt = "The rain in Spain"
x = re.search("\s", txt)

print("The first white-space character is located in position:", x.start())
Se nenhuma correspondência for encontrada, o valor Noneserá retornado:

Exemplo
Faça uma pesquisa que não retorne nenhuma correspondência:

import re

txt = "The rain in Spain"
x = re.search("Portugal", txt)
print(x)
 
A função split()
A split()função retorna uma lista onde a string foi dividida em cada correspondência:

Exemplo
Dividir em cada caractere de espaço em branco:

import re

txt = "The rain in Spain"
x = re.split("\s", txt)
print(x)
Você pode controlar o número de ocorrências especificando o maxsplit parâmetro:

Exemplo
Divida a string apenas na primeira ocorrência:

import re

txt = "The rain in Spain"
x = re.split("\s", txt, 1)
print(x)
 
A função sub()
A sub()função substitui as correspondências pelo texto de sua escolha:

Exemplo
Substitua cada caractere de espaço em branco pelo número 9:

import re

txt = "The rain in Spain"
x = re.sub("\s", "9", txt)
print(x)
Você pode controlar o número de substituições especificando o count parâmetro:

Exemplo
Substitua as 2 primeiras ocorrências:

import re

txt = "The rain in Spain"
x = re.sub("\s", "9", txt, 2)
print(x)
 
Objeto de correspondência
Um Match Object é um objeto que contém informações sobre a pesquisa e o resultado.

Nota: Se não houver correspondência, o valor Noneserá retornado, em vez do Objeto de correspondência.

Exemplo
Faça uma pesquisa que retornará um Match Object:

import re

txt = "The rain in Spain"
x = re.search("ai", txt)
print(x) #this will print an object
O objeto Match possui propriedades e métodos usados ​​para recuperar informações sobre a pesquisa e o resultado:

.span()retorna uma tupla contendo as posições inicial e final da correspondência.
.stringretorna a string passada para a função
.group()retorna a parte da string onde houve uma correspondência
Exemplo
Imprima a posição (posição inicial e final) da primeira ocorrência de correspondência.

A expressão regular procura qualquer palavra que comece com "S" maiúsculo:

import re

txt = "The rain in Spain"
x = re.search(r"\bS\w+", txt)
print(x.span())
Exemplo
Imprima a string passada na função:

import re

txt = "The rain in Spain"
x = re.search(r"\bS\w+", txt)
print(x.string)
Exemplo
Imprima a parte da string onde houve uma correspondência.

A expressão regular procura qualquer palavra que comece com "S" maiúsculo:

import re

txt = "The rain in Spain"
x = re.search(r"\bS\w+", txt)
print(x.group())
Nota: Se não houver correspondência, o valor Noneserá retornado, em vez do Objeto de correspondência.