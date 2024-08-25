# ExCaixa
 Primeiro Repositório

saldo = 1000.00

while True:
    
    print("\nCaixa Eletronico")
    print("1 - Verificar Saldo")
    print("2 - Depositar dinheiro")
    print("3 - Sacar Dinheiro")
    print("4 - Sair")
    
    opcao = input("Escolha a opção:")
    
    if opcao == "1":
        
        print(f"Seu saldo: R${saldo:.2f}")
        
    elif opcao == "2":
        
        deposito = float(input("Digite o valor do depósito: R$ "))
        
        if deposito > 0:
            
            saldo += deposito
            
            print(f"Depósito de: R$ {deposito:.2f} realizado com sucesso!")
            
        else:
            
            print(f"Valor de depósito inválido")
            
    elif opcao == "3":
        
        saque = float(input("Digite o valor do saque: R$ "))
        
        if saque > 0 and saque <= saldo:
            
            saldo -= saque
            
            print(f"Saque de: R$ {saque:.2f} realizado com sucesso!")
            
        else:
            
            print(f"Valor do saque inválido ou saldo insuficiente")
            
    elif opcao == "4":
     
        print ("Obrigado por utilizar o nosso caixa eletrônico.")
        
        break
    
    else:
        print("Opção invalida. Por favor, tente novamente!")
    