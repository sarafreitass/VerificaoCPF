# Verifica-o-de-CPF
algoritmo que verifica a validade de um CPF
CPF= abc.def.ghi-jk

PRIMEIRA PARTE                         SEGUNDA PARTE
a * n   = r0                         a * n+1 = r0
b * n-1 = r1                         b * n   = r1
c * ... = r2                         c * n-1 = r2
d * ... = r3                         d * ... = r3
e * ... = r4                         e * ... = r4
f * ... = r5                         f * ... = r5
g * ... = r6                         g * ... = r6
h * ... = r7                         h * ... = r7
i * n-8 = r8                         i * ... = r8
                                     j * n-8 = r9

soma final = r0 + ... + r8           soma final = r0 + ... + r9

11 - (soma final % 11) = rf          11 - (soma final % 11) = rf

rf>9 == true (digito1=0)             rf>9 == true (digito2=0)
rf<=9 == true (digito1=rf)           rf<=9 == true (digito2=rf)


para obter o primeiro digito depois do traço,
pega os nove primeiros numeros e
multiplica por um contagem regressiva
depois soma todos os resultados
ai voce pega 11 e subtrai pelo resto do modulo da soma com 11
se esse resultado for maior do que 9, o digito vai ser 0

NO FINAL O CPF DADO E O CPF GERADO PELO SISTEMA COM OS DOIS
DIGITOS PRECISAM SER IGUAIS PARA ESTAR VALIDADO
