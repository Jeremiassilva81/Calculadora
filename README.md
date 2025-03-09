# Calculadora
def calcular():
    print("Calculadora Simples")
    print("Escolha a operação:")
    print("1 - Adição")
    print("2 - Subtração")
    print("3 - Multiplicação")
    print("4 - Divisão")
    
    opcao = input("Digite o número da operação desejada: ")
    
    if opcao not in ('1', '2', '3', '4'):
        print("Opção inválida! Tente novamente.")
        return
    
    num1 = float(input("Digite o primeiro número: "))
    num2 = float(input("Digite o segundo número: "))
    
    if opcao == '1':
        print(f"Resultado: {num1 + num2}")
    elif opcao == '2':
        print(f"Resultado: {num1 - num2}")
    elif opcao == '3':
        print(f"Resultado: {num1 * num2}")
    elif opcao == '4':
        if num2 == 0:
            print("Erro! Divisão por zero não permitida.")
        else:
            print(f"Resultado: {num1 / num2}")

if __name__ == "__main__":
    calcular()
