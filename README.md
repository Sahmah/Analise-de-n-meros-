#Seletores de Elementos HTML:

O código começa selecionando os elementos HTML que serão utilizados:
num: O campo de entrada onde o usuário digita um número.
lista: A lista de opções que será exibida com os números adicionados.
res: A área onde os resultados das operações (soma, média, etc.) serão exibidos.
valores: Um array vazio que armazenará os números inseridos.

Função isNumero(n):
Objetivo: Verificar se o número inserido está dentro do intervalo de 1 a 100.
Se o número for maior ou igual a 1 e menor ou igual a 100, a função retorna true; caso contrário, retorna false.

Função inLista(n, I):
Objetivo: Verificar se o número inserido já existe na lista de números.
A função retorna true se o número já estiver na lista (usando o método indexOf()), e false caso contrário.

Função adicionar():
Objetivo: Adicionar o número digitado à lista, se ele for válido e não estiver repetido.
Primeiro, verifica se o número é válido (usando a função isNumero()) e se ainda não foi adicionado à lista (usando a função inLista()).
Se o número for válido, ele é adicionado ao array valores e um item de lista (<option>) é criado para mostrar ao usuário que o valor foi adicionado.
Caso o número seja inválido ou já tenha sido inserido, um alerta é exibido para informar o erro.
Após adicionar ou não o número, o campo de entrada é limpo e o foco é reposicionado para que o usuário possa digitar o próximo número.

Função finalizar():
Objetivo: Realizar os cálculos e exibir os resultados, como total de números, maior valor, menor valor, soma e média.
Antes de realizar os cálculos, verifica se algum número foi adicionado à lista. Se não houver números, um alerta é exibido.
Caso haja números, o código segue com os cálculos:
Total de números: Calculado pela quantidade de elementos no array valores.
Maior e menor valor: Inicializa com o primeiro número e compara os demais para encontrar os maiores e menores valores.
Soma: Soma todos os valores inseridos.
Média: Calcula a média dividindo a soma pelo total de números.
Após os cálculos, os resultados são exibidos no elemento res, com as informações formatadas.
