Introdução ao Python
O que é Python?
Python é uma linguagem de programação popular. Foi criado por Guido van Rossum e lançado em 1991.

É usado para:

desenvolvimento web (lado do servidor),
desenvolvimento de software,
matemática,
script do sistema.

O que o Python pode fazer?
Python pode ser usado em um servidor para criar aplicativos da web.
O Python pode ser usado junto com o software para criar fluxos de trabalho.
Python pode se conectar a sistemas de banco de dados. Ele também pode ler e modificar arquivos.
Python pode ser usado para lidar com big data e realizar matemática complexa.
Python pode ser usado para prototipagem rápida ou para desenvolvimento de software pronto para produção.
Por que Python?
Python funciona em diferentes plataformas (Windows, Mac, Linux, Raspberry Pi, etc).
Python tem uma sintaxe simples semelhante ao idioma inglês.
Python tem sintaxe que permite aos desenvolvedores escrever programas com menos linhas do que algumas outras linguagens de programação.
Python é executado em um sistema interpretador, o que significa que o código pode ser executado assim que for escrito. Isso significa que a prototipagem pode ser muito rápida.
Python pode ser tratado de forma procedural, orientada a objetos ou funcional.
Bom saber
A versão principal mais recente do Python é o Python 3, que usaremos neste tutorial. No entanto, o Python 2, embora não seja atualizado com nada além de atualizações de segurança, ainda é bastante popular.
Neste tutorial Python será escrito em um editor de texto. É possível escrever Python em um ambiente de desenvolvimento integrado, como Thonny, Pycharm, Netbeans ou Eclipse, que são particularmente úteis ao gerenciar coleções maiores de arquivos Python.
Sintaxe do Python em comparação com outras linguagens de programação
O Python foi projetado para facilitar a leitura e possui algumas semelhanças com o idioma inglês com influência da matemática.
Python usa novas linhas para completar um comando, ao contrário de outras linguagens de programação que geralmente usam ponto e vírgula ou parênteses.
Python depende de recuo, usando espaço em branco, para definir o escopo; como o escopo de loops, funções e classes. Outras linguagens de programação costumam usar colchetes para essa finalidade.
Exemplo
print("Hello, World!")

Introdução ao Python
Instalação do Python
Muitos PCs e Macs terão o python já instalado.

Para verificar se você tem o python instalado em um PC com Windows, pesquise na barra inicial por Python ou execute o seguinte na linha de comando (cmd.exe):

C:\Users\Your Name>python --version
Para verificar se você tem o python instalado em um Linux ou Mac, então no linux abra a linha de comando ou no Mac abra o Terminal e digite:

python --version
Se você achar que não tem o Python instalado em seu computador, você pode baixá-lo gratuitamente no seguinte site: https://www.python.org/

Guia de início rápido do Python
Python é uma linguagem de programação interpretada, isso significa que, como desenvolvedor, você escreve arquivos Python (.py) em um editor de texto e depois coloca esses arquivos no interpretador python para serem executados.

A maneira de executar um arquivo python é assim na linha de comando:

C:\Users\Your Name>python helloworld.py
Onde "helloworld.py" é o nome do seu arquivo python.

Vamos escrever nosso primeiro arquivo Python, chamado helloworld.py, que pode ser feito em qualquer editor de texto.

helloworld.py

print("Hello, World!")
Simples assim. Salve seu arquivo. Abra sua linha de comando, navegue até o diretório onde você salvou seu arquivo e execute:

C:\Users\Your Name>python helloworld.py
A saída deve ser:

Hello, World!
Parabéns, você escreveu e executou seu primeiro programa Python.

A linha de comando do Python
Para testar uma pequena quantidade de código em python, às vezes é mais rápido e fácil não escrever o código em um arquivo. Isso é possível porque o Python pode ser executado como uma linha de comando.

Digite o seguinte na linha de comando do Windows, Mac ou Linux:

C:\Users\Your Name>python
Ou, se o comando "python" não funcionou, você pode tentar "py":
C:\Users\Your Name>py
A partir daí, você pode escrever qualquer python, incluindo nosso exemplo hello world do início do tutorial:

C:\Users\Your Name>python
Python 3.6.4 (v3.6.4:d48eceb, Dec 19 2017, 06:04:45) [MSC v.1900 32 bit (Intel)] on win32
Type "help", "copyright", "credits" or "license" for more information.
>>> print("Hello, World!")
Que escreverá "Hello, World!" na linha de comando:

C:\Users\Your Name>python
Python 3.6.4 (v3.6.4:d48eceb, Dec 19 2017, 06:04:45) [MSC v.1900 32 bit (Intel)] on win32
Type "help", "copyright", "credits" or "license" for more information.
>>> print("Hello, World!")
Hello, World!
Sempre que você terminar na linha de comando do python, você pode simplesmente digitar o seguinte para sair da interface da linha de comando do python:

exit()
