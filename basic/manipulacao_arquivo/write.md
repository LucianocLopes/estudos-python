Gravação de arquivo Python
Gravar em um arquivo existente
Para gravar em um arquivo existente, você deve adicionar um parâmetro à open()função:

"a"- Append - anexará ao final do arquivo

"w"- Write - substituirá qualquer conteúdo existente

Exemplo
Abra o arquivo "demofile2.txt" e anexe o conteúdo ao arquivo:

f = open("demofile2.txt", "a")
f.write("Now the file has more content!")
f.close()

#open and read the file after the appending:
f = open("demofile2.txt", "r")
print(f.read())
Exemplo
Abra o arquivo "demofile3.txt" e sobrescreva o conteúdo:

f = open("demofile3.txt", "w")
f.write("Woops! I have deleted the content!")
f.close()

#open and read the file after the appending:
f = open("demofile3.txt", "r")
print(f.read())
Nota: o método "w" substituirá o arquivo inteiro.

Criar um novo arquivo
Para criar um novo arquivo em Python, use o open()método, com um dos seguintes parâmetros:

"x"- Criar - criará um arquivo, retornará um erro se o arquivo existir

"a"- Append - criará um arquivo se o arquivo especificado não existir

"w"- Write - criará um arquivo se o arquivo especificado não existir

Exemplo
Crie um arquivo chamado "meuarquivo.txt":

f = open("myfile.txt", "x")
Resultado: um novo arquivo vazio é criado!

Exemplo
Crie um novo arquivo se ele não existir:

f = open("myfile.txt", "w")