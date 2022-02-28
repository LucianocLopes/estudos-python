Arquivo Python aberto
Abra um arquivo no servidor
Suponha que temos o seguinte arquivo, localizado na mesma pasta do Python:

demofile.txt

Hello! Welcome to demofile.txt
This file is for testing purposes.
Good Luck!
Para abrir o arquivo, use a open()função interna.

A open()função retorna um objeto de arquivo, que possui um read()método para leitura do conteúdo do arquivo:

Exemplo
f = open("demofile.txt", "r")
print(f.read())
Se o arquivo estiver localizado em um local diferente, você terá que especificar o caminho do arquivo, assim:

Exemplo
Abra um arquivo em um local diferente:

f = open("D:\\myfiles\welcome.txt", "r")
print(f.read())
Somente leitura de partes do arquivo
Por padrão, o read()método retorna o texto inteiro, mas você também pode especificar quantos caracteres deseja retornar:

Exemplo
Retorne os 5 primeiros caracteres do arquivo:

f = open("demofile.txt", "r")
print(f.read(5))
PROPAGANDA

Linhas de leitura
Você pode retornar uma linha usando o readline()método:

Exemplo
Leia uma linha do arquivo:

f = open("demofile.txt", "r")
print(f.readline())
Ao ligar readline()duas vezes, você pode ler as duas primeiras linhas:

Exemplo
Leia duas linhas do arquivo:

f = open("demofile.txt", "r")
print(f.readline())
print(f.readline())
Fazendo um loop pelas linhas do arquivo, você pode ler o arquivo inteiro, linha por linha:

Exemplo
Percorra o arquivo linha por linha:

f = open("demofile.txt", "r")
for x in f:
  print(x)
Fechar arquivos
É uma boa prática sempre fechar o arquivo quando terminar.

Exemplo
Feche o arquivo quando terminar com ele:

f = open("demofile.txt", "r")
print(f.readline())
f.close()
Nota: Você deve sempre fechar seus arquivos, em alguns casos, devido ao buffer, as alterações feitas em um arquivo podem não aparecer até que você feche o arquivo.