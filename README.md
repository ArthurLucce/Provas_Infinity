# Solicita os limites do intervalo ao usuário
inicio = int(input("Digite o número inicial do intervalo: "))
fim = int(input("Digite o número final do intervalo: "))

soma_pares = 0
tem_par = False

# Itera sobre o intervalo incluindo o número final
for numero in range(inicio, fim + 1):
    if numero % 2 == 0:
        soma_pares += numero
        tem_par = True
else:
    if tem_par:
        print(f"A soma dos números pares no intervalo de {inicio} a {fim} é: {soma_pares}")
    else:
        print(f"Não há números pares no intervalo de {inicio} a {fim}.")
