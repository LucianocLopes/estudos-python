Matemática Python
O Python possui um conjunto de funções matemáticas integradas, incluindo um extenso módulo matemático, que permite realizar tarefas matemáticas em números.

Funções matemáticas incorporadas
As funções min()e max()podem ser usadas para encontrar o valor mais baixo ou mais alto em um iterável:

Exemplo
x = min(5, 10, 25)
y = max(5, 10, 25)

print(x)
print(y)
A abs()função retorna o valor absoluto (positivo) do número especificado:

Exemplo
x = abs(-7.25)

print(x)
A função retorna o valor de x elevado à potência de y (x y ).pow(x, y)

Exemplo
Retorne o valor de 4 à potência de 3 (o mesmo que 4 * 4 * 4):

x = pow(4, 3)

print(x)
PROPAGANDA

O módulo de matemática
Python também tem um módulo embutido chamado math, que estende a lista de funções matemáticas.

Para usá-lo, você deve importar o mathmódulo:

import math
Depois de importar o mathmódulo, você pode começar a usar métodos e constantes do módulo.

O math.sqrt()método, por exemplo, retorna a raiz quadrada de um número:

Exemplo
import math

x = math.sqrt(64)

print(x)
O math.ceil()método arredonda um número para cima até o número inteiro mais próximo e o math.floor() método arredonda um número para baixo até o número inteiro mais próximo e retorna o resultado:

Exemplo
import math

x = math.ceil(1.4)
y = math.floor(1.4)

print(x) # returns 2
print(y) # returns 1
A math.piconstante, retorna o valor de PI (3.14...):

Exemplo
import math

x = math.pi

print(x)
Referência Completa do Módulo de Matemática
Em nosso Math Module Reference você encontrará uma referência completa de todos os métodos e constantes que pertencem ao módulo Math.