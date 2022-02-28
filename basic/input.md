Entrada do usuário Python
Entrada do usuário
Python permite a entrada do usuário.

Isso significa que podemos solicitar a entrada do usuário.

O método é um pouco diferente no Python 3.6 do Python 2.7.

Python 3.6 usa o input()método.

Python 2.7 usa o raw_input()método.

O exemplo a seguir solicita o nome de usuário e, quando você digita o nome de usuário, ele é impresso na tela:

Python 3.6
username = input("Enter username:")
print("Username is: " + username)
Python 2.7
username = raw_input("Enter username:")
print("Username is: " + username)
O Python para de executar quando se trata da input()função e continua quando o usuário fornece alguma entrada.