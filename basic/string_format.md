Formatação de String Python
Para garantir que uma string seja exibida conforme o esperado, podemos formatar o resultado com o format()método.

Formato de string()
O format()método permite formatar partes selecionadas de uma string.

Às vezes, há partes de um texto que você não controla, talvez venham de um banco de dados ou de uma entrada do usuário?

Para controlar esses valores, adicione espaços reservados (colchetes {}) no texto e execute os valores pelo format()método:

Exemplo
Adicione um espaço reservado onde você deseja exibir o preço:

price = 49
txt = "The price is {} dollars"
print(txt.format(price))
Você pode adicionar parâmetros dentro das chaves para especificar como converter o valor:

Exemplo
Formate o preço a ser exibido como um número com duas casas decimais:

txt = "The price is {:.2f} dollars"
Confira todos os tipos de formatação em nossa String format() Reference .

Vários valores
Se você quiser usar mais valores, basta adicionar mais valores ao método format():

print(txt.format(price, itemno, count))
E adicione mais espaços reservados:

Exemplo
quantity = 3
itemno = 567
price = 49
myorder = "I want {} pieces of item number {} for {:.2f} dollars."
print(myorder.format(quantity, itemno, price))
ADVERTISEMENT

Números de índice
Você pode usar números de índice (um número dentro das chaves {0}) para garantir que os valores sejam colocados nos espaços reservados corretos:

Exemplo
quantity = 3
itemno = 567
price = 49
myorder = "I want {0} pieces of item number {1} for {2:.2f} dollars."
print(myorder.format(quantity, itemno, price))
Além disso, se você quiser fazer referência ao mesmo valor mais de uma vez, use o número de índice:

Exemplo
age = 36
name = "John"
txt = "His name is {1}. {1} is {0} years old."
print(txt.format(age, name))
Índices nomeados
Você também pode usar índices nomeados inserindo um nome dentro das chaves {carname}, mas você deve usar nomes ao passar os valores dos parâmetros txt.format(carname = "Ford"):

Exemplo
myorder = "I have a {carname}, it is a {model}."
print(myorder.format(carname = "Ford", model = "Mustang"))