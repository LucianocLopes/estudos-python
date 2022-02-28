Python PIP
O que é o PIP?
PIP é um gerenciador de pacotes para pacotes Python, ou módulos, se preferir.

Observação: se você tiver o Python versão 3.4 ou posterior, o PIP será incluído por padrão.

O que é um Pacote?
Um pacote contém todos os arquivos necessários para um módulo.

Módulos são bibliotecas de código Python que você pode incluir em seu projeto.

Verifique se o PIP está instalado
Navegue pela linha de comando até o local do diretório de scripts do Python e digite o seguinte:

Exemplo
Verifique a versão do PIP:

C:\Users\Your Name\AppData\Local\Programs\Python\Python36-32\Scripts>pip --version
Instalar PIP
Se você não tiver o PIP instalado, poderá baixá-lo e instalá-lo nesta página: https://pypi.org/project/pip/

Baixar um pacote
Baixar um pacote é muito fácil.

Abra a interface de linha de comando e diga ao PIP para baixar o pacote desejado.

Navegue pela linha de comando até o local do diretório de scripts do Python e digite o seguinte:

Exemplo
Baixe um pacote chamado "camelcase":

C:\Users\Your Name\AppData\Local\Programs\Python\Python36-32\Scripts>pip install camelcase
Agora você baixou e instalou seu primeiro pacote!

PROPAGANDA

Usando um pacote
Uma vez que o pacote está instalado, ele está pronto para uso.

Importe o pacote "camelcase" para o seu projeto.

Exemplo
Importe e use "camelcase":

import camelcase

c = camelcase.CamelCase()

txt = "hello world"

print(c.hump(txt))
Encontrar pacotes
Encontre mais pacotes em https://pypi.org/ .

Remover um pacote
Use o uninstallcomando para remover um pacote:

Exemplo
Desinstale o pacote chamado "camelcase":

C:\Users\Your Name\AppData\Local\Programs\Python\Python36-32\Scripts>pip uninstall camelcase
O Gerenciador de Pacotes PIP solicitará que você confirme se deseja remover o pacote camelcase:

Uninstalling camelcase-02.1:
  Would remove:
    c:\users\Your Name\appdata\local\programs\python\python36-32\lib\site-packages\camecase-0.2-py3.6.egg-info
    c:\users\Your Name\appdata\local\programs\python\python36-32\lib\site-packages\camecase\*
Proceed (y/n)?
Pressione ye o pacote será removido.

Listar pacotes
Use o listcomando para listar todos os pacotes instalados em seu sistema:

Exemplo
Listar os pacotes instalados:

C:\Users\Your Name\AppData\Local\Programs\Python\Python36-32\Scripts>pip list
Resultado:

Package         Version
-----------------------
camelcase       0.2
mysql-connector 2.1.6
pip             18.1
pymongo         3.6.1
setuptools      39.0.1