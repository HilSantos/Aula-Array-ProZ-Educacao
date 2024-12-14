# Aula-Array-ProZ-Educacao
Definir uma função com dois parâmetros; percorrer um array e alterar uma variável booleana caso encontrar o elemento; imprimir uma mensagem avisando que o elemento foi encontrado ou não; definir um array e testar a função. Fazer com que o sistema pergunte ao usuário o elemento que deseja a procurar, e continue perguntando até achar um.

def achar_elemento(elem, arr):
  boole = False
  for i in range(len(arr)):
    if arr[i] == elem:
      boole = True
  if (boole == False):
    print("Não achamos o nome " + elem)
  else:
    print("Achamos o nome " + elem)
      
nomes = ["hilton", "carol", "joão", "líniker"]
achar_elemento("jana" , nomes)

def achar_elemento(arr):
  boole = False
  while(boole == False):
    elem = input("digite um nome: ")
    for i in range(len(arr)):
      if arr[i] == elem:
        boole = True
    if (boole == False):
      print("Não achamos o nome: " + elem)
    else:
      print("Achamos o nome: " + elem)
      
nomes = ["hilton", "carol", "joão", "líniker"]
achar_elemento(nomes)
