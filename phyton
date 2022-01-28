                                        #PEGAR ENTRADA

cpf_original = input("Digite seu CPF: ")
#cpf_original = "51504690842"

    #precisa transformar a entrada em uma lista de numeros
    #para isso você pode separar cada item da string e colocar dentro de um
    #laço para converter cada um em numero

    #separação de cada item da string
cpf_lista = []
cpf_final = []     ##
for i in range(0,len(cpf_original),1):
    cpf_lista.append(cpf_original[i])
    cpf_final.append(cpf_original[i])    ##
    i+=1

#print(cpf_lista)

    #laço para converter tudo em números, transforma a string do cpf_original
    #em uma lista de números chamada cpf_lista
for i in range(0,len(cpf_lista),1):
    cpf_lista[i] = int(cpf_lista[i])
    cpf_final[i] = cpf_lista[i]     ##
    i+=1

#print(cpf_lista)
                            #CRIAR CPF SEM DIGITOS FINAIS (para fazer a comparação)
cpf_gerado = cpf_lista
del (cpf_gerado[10])
del (cpf_gerado[9])

#print(cpf_gerado)

                                            #MULTIPLICAÇÃO (digito1)

n = int(input("Digite o número máximo para o começo da multiplicação: "))
#n = 10
a = n
lista_mult = []

for s in range(0, 9):
    lista_mult.append(cpf_gerado[s]*a)
    a-=1

#print(lista_mult)

                                        #DETERMINAÇÃO DO DÍGITO 1

#print(sum(lista_mult))

resultado = 11 - (sum(lista_mult) % 11)

if resultado>9:
    digito1 = 0
else:
    digito1 = resultado

#print(digito1)

                                    #ACRESCENTAR PRIMEIRO DIGITO AO cpf_gerado

cpf_gerado.append(digito1)
#print(cpf_gerado)

                                            #MULTIPLICAÇÃO (digito2)

n = n + 1
a = n
lista_mult = []

for s in range(0, 10):
    lista_mult.append(cpf_gerado[s]*a)
    a-=1

#print(lista_mult)

                                        #DETERMINAÇÃO DO DÍGITO 2

#print(sum(lista_mult))

resultado = 11 - (sum(lista_mult) % 11)

if resultado>9:
    digito2 = 0
else:
    digito2 = resultado

#print(digito2)

                                    #ACRESCENTAR PRIMEIRO DIGITO AO cpf_gerado

cpf_gerado.append(digito2)
#print(cpf_gerado)


                                            #VERIFICAÇÃO DO CPF
    #o Set é uma coleção de elementos e não está ordenado.
    #podemos converter diretamente uma lista em um conjunto usando a função set() e compará-los por igualdade.

print(cpf_gerado)
print(cpf_final)

if (set(cpf_gerado)==set(cpf_final)):
    print('O CPF é válido!')
else:
    print('O CPF é inválido :(')
