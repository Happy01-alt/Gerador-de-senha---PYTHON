import random
import string

print("Bem-vindo ao gerador de senhas!\n Irei criar uma senha para você.\n A senha terá automaticamente letras maiúsculas e minúsculas.")

pergunta = input("Quer que esta senha tenha números? (s/n)\n")

letras = string.ascii_letters + string.digits

amanho = input("Qual será o tamanho da senha?\n")

senha = ''.join(random.choice(letras) for i in range(int(tamanho)))

print("Senha gerada:", senha)
guardar = input("Deseja guardar a senha em um arquivo? (s/n)\n")
if guardar.lower() == 's':
    with open(r"C:\Users\user\Desktop\senha.txt", "a") as arquivo:
            arquivo.write(senha)
                print("Senha guardada em senhas.txt")
