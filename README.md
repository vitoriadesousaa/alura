# Definindo o número secreto
numero_secreto = 7 

print("Tente adivinhar o número secreto entre 1 e 10!")

# Loop para 5 tentativas
for tentativa in range(1, 6):
    palpite = int(input(f"Tentativa {tentativa}: Digite seu palpite: "))

    if palpite == numero_secreto:
        print("Parabéns")
        break
    elif palpite < numero_secreto:
        print("Muito baixo!")
    else:
        print("Muito alto!")
else:
    # Executado se o loop terminar sem o break
    print(f"Você perdeu! O número correto era {numero_secreto}.")
