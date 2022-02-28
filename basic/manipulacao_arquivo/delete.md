Arquivo Excluir Python
Excluir um arquivo
Para excluir um arquivo, você deve importar o módulo do SO e executar sua os.remove()função:

Exemplo
Remova o arquivo "demofile.txt":

import os
os.remove("demofile.txt")
Verifique se o arquivo existe:
Para evitar erros, verifique se o arquivo existe antes de tentar excluí-lo:

Exemplo
Verifique se o arquivo existe e exclua-o:

import os
if os.path.exists("demofile.txt"):
  os.remove("demofile.txt")
else:
  print("The file does not exist")
Excluir pasta
Para excluir uma pasta inteira, use o os.rmdir()método:

Exemplo
Remova a pasta "minhapasta":

import os
os.rmdir("myfolder")
Nota: Você só pode remover pastas vazias .