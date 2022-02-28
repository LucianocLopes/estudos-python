Comentários do Python
Os comentários podem ser usados ​​para explicar o código Python.

Comentários podem ser usados ​​para tornar o código mais legível.

Os comentários podem ser usados ​​para impedir a execução ao testar o código.

Criando um comentário
Os comentários começam com #, e o Python os ignorará:

Exemplo
#This is a comment
print("Hello, World!")
Os comentários podem ser colocados no final de uma linha e o Python ignorará o resto da linha:

Exemplo
print("Hello, World!") #This is a comment
Um comentário não precisa ser um texto que explique o código, ele também pode ser usado para impedir que o Python execute o código:

Exemplo
#print("Hello, World!")
print("Cheers, Mate!")

Comentários de várias linhas
O Python realmente não possui uma sintaxe para comentários de várias linhas.

Para adicionar um comentário de várias linhas, você pode inserir um #para cada linha:

Exemplo
#This is a comment
#written in
#more than just one line
print("Hello, World!")
Ou, não exatamente como pretendido, você pode usar uma string de várias linhas.

Como o Python ignorará literais de string que não são atribuídos a uma variável, você pode adicionar uma string de várias linhas (aspas triplas) em seu código e colocar seu comentário dentro dela:

Exemplo
"""
This is a comment
written in
more than just one line
"""
print("Hello, World!")
Contanto que a string não seja atribuída a uma variável, o Python lerá o código, mas o ignorará e você fez um comentário de várias linhas.