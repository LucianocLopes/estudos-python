Arquivo Python aberto
O manuseio de arquivos é uma parte importante de qualquer aplicativo da web.

Python tem várias funções para criar, ler, atualizar e deletar arquivos.

Manipulação de arquivos
A função chave para trabalhar com arquivos em Python é a open()função.

A open()função recebe dois parâmetros; nome do arquivo e modo .

Existem quatro métodos (modos) diferentes para abrir um arquivo:

"r"- Leitura - Valor padrão. Abre um arquivo para leitura, erro se o arquivo não existir

"a"- Append - Abre um arquivo para anexação, cria o arquivo se não existir

"w"- Write - Abre um arquivo para escrita, cria o arquivo caso não exista

"x"- Criar - Cria o arquivo especificado, retorna um erro se o arquivo existir

Além disso você pode especificar se o arquivo deve ser tratado como modo binário ou texto

"t"- Texto - Valor padrão. Modo de texto

"b"- Binário - Modo binário (por exemplo, imagens)

Sintaxe
Para abrir um arquivo para leitura, basta especificar o nome do arquivo:

f = open("demofile.txt")
O código acima é o mesmo que:

f = open("demofile.txt", "rt")
Como "r"para leitura e "t"para texto são os valores padrão, você não precisa especificá-los.

Nota: Certifique-se de que o arquivo existe, caso contrário você receberá um erro.