Operadores Python
Operadores Python
Os operadores são usados ​​para realizar operações em variáveis ​​e valores.

No exemplo abaixo, usamos o +operador para somar dois valores:

Exemplo
print(10 + 5)
Python divide os operadores nos seguintes grupos:

Operadores aritméticos
Operadores de atribuição
Operadores de comparação
Operadores lógicos
Operadores de identidade
Operadores de associação
Operadores bit a bit
Operadores aritméticos Python
Os operadores aritméticos são usados ​​com valores numéricos para realizar operações matemáticas comuns:

Operator	Name	Example	Try it
+	Addition	x + y	
-	Subtraction	x - y	
*	Multiplication	x * y	
/	Division	x / y	
%	Modulus	x % y	
**	Exponentiation	x ** y	
//	Floor division	x // y	
Operadores de atribuição Python
Os operadores de atribuição são usados ​​para atribuir valores a variáveis:

Operator	Example	Same As	Try it
=	x = 5	x = 5	
+=	x += 3	x = x + 3	
-=	x -= 3	x = x - 3	
*=	x *= 3	x = x * 3	
/=	x /= 3	x = x / 3	
%=	x %= 3	x = x % 3	
//=	x //= 3	x = x // 3	
**=	x **= 3	x = x ** 3	
&=	x &= 3	x = x & 3	
|=	x |= 3	x = x | 3	
^=	x ^= 3	x = x ^ 3	
>>=	x >>= 3	x = x >> 3	
<<=	x <<= 3	x = x << 3	
PROPAGANDA

Operadores de comparação Python
Os operadores de comparação são usados ​​para comparar dois valores:

Operator	Name	Example	Try it
==	Equal	x == y	
!=	Not equal	x != y	
>	Greater than	x > y	
<	Less than	x < y	
>=	Greater than or equal to	x >= y	
<=	Less than or equal to	x <= y	
Operadores lógicos Python
Os operadores lógicos são usados ​​para combinar instruções condicionais:

Operator	Description	Example	Try it
and 	Returns True if both statements are true	x < 5 and  x < 10	
or	Returns True if one of the statements is true	x < 5 or x < 4	
not	Reverse the result, returns False if the result is true	not(x < 5 and x < 10)	
Operadores de identidade Python
Os operadores de identidade são usados ​​para comparar os objetos, não se forem iguais, mas se forem realmente o mesmo objeto, com a mesma localização de memória:

Operator	Description	Example	Try it
is 	Returns True if both variables are the same object	x is y	
is not	Returns True if both variables are not the same object	x is not y	
Operadores de associação Python
Os operadores de associação são usados ​​para testar se uma sequência é apresentada em um objeto:

Operator	Description	Example	Try it
in 	Returns True if a sequence with the specified value is present in the object	x in y	
not in	Returns True if a sequence with the specified value is not present in the object	x not in y	
Operadores Bitwise Python
Operadores bit a bit são usados ​​para comparar números (binários):

Operator	Name	Description
& 	AND	Sets each bit to 1 if both bits are 1
|	OR	Sets each bit to 1 if one of two bits is 1
 ^	XOR	Sets each bit to 1 if only one of two bits is 1
~ 	NOT	Inverts all the bits
<<	Zero fill left shift	Shift left by pushing zeros in from the right and let the leftmost bits fall off
>>	Signed right shift	Shift right by pushing copies of the leftmost bit in from the left, and let the rightmost bits fall off