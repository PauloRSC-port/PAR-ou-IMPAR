import random
print("----- VAMOS JOGAR PAR OU ÍMPAR -----")
pc = random.randint(1,11)
maq = 'PAR', 'IMPAR'
perg = 'PAR', 'IMPAR' 
user = soma = resultado = 0
win = 0
while True:
    perg = str(input("Escolha PAR ou ÍMPAR:  ")).strip().upper()
    if perg not in ['PAR', 'IMPAR']:
        print("----- ESCOLHA INVÁLIDA -----\nEscolha entre PAR OU ÍMPAR.")
        perg = str(input("Escolha PAR ou ÍMPAR:  ")).strip().upper()
    user = int(input("Agora escolha um número: "))
    soma += user + pc
    win += 1
    if perg == 'PAR':
        maq == 'ÍMPAR'
        if soma % 2 == 0:
            print(f"Sua escolha foi {user} e a máquina escolheu {pc}.")
            print(f"VOCÊ VENCEU!!!!\nEssa é sua quantidade de vitórias {win}.")
        elif soma % 2 == 1:
            print(f"Sua escolha foi {user} e a máquina escolheu {pc}.")
            print("A máquina VENCEU!!!! HAHAHAHAHAHA")
            break             
    elif perg == 'IMPAR':
        maq == 'PAR'
        if soma % 2 == 0:
            print(f"Sua escolha foi {user} e a máquina escolheu {pc}.")
            print("A máquina VENCEU!!!! HAHAHAHAHAHA")
            break
        elif soma % 2 == 1:
            print(f"Sua escolha foi {user} e a máquina escolheu {pc}.")
            print(f"VOCÊ VENCEU!!!!\nEssa é sua quantidade de vitórias {win}.")
print("-=-=-=-=-=- FIM -=-=-=-=-=-")            
            


