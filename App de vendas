print("Boas vindas ao app de vendas criado por Nicoly")

#Define o menu de opções
def menu():
    print("Cardápio de Açaí e Cupuaçu")
    print("Tamanho P de Cupuaçu (CP) custa R$ 9.00 e o Açaí (AC) custa R$ 11.00")
    print("Tamanho M de Cupuaçu (CP) custa R$ 14.00 e o Açaí (AC) custa R$ 16.00")
    print("Tamanho G de Cupuaçu (CP) custa R$ 18.00 e o Açaí (AC) custa R$ 20.00")

# Escolhe o sabor e tamanho do pedido no input, caso não tenha a opção traz inválido
def sabor_tamanho():
    menu()
    print("Selecione o sabor desejado:\nCupuaçu (CP)\nAçaí (AC)")
    sabor = input("Escolha o sabor: (CP para Cupuaçu e AC para Açaí)").strip().upper()
    if sabor not in ['CP', 'AC']:
        print("Sabor inválido, tente novamente!")
        sabor_tamanho()
                  
    print("Selecione o tamanho desejado:\nTamanho P\nTamanho M\nTamanho G")
    tamanho = input("Escolha o tamanho:").strip().upper()
    if tamanho not in ['P', 'M', 'G']:
        print("Tamanho inválido, tente novamente!")
        sabor_tamanho()
    
    return sabor, tamanho

# Função que traz o valor do pedido com base no sabor e tamanho e retorna o print do pedido e valor
def realizar_pedido():
    sabor, tamanho = sabor_tamanho()
    
    if sabor == "CP":
        if tamanho == "P":
            preco_pedido = 9.00
        elif tamanho == "M":
            preco_pedido = 14.00
        else:
            preco_pedido = 18.00
    elif sabor == "AC":
        if tamanho == "P":
            preco_pedido = 11.00
        elif tamanho == "M":
            preco_pedido = 16.00
        else:
            preco_pedido = 20.00
    print(f"Pedido realizado: {sabor} - {tamanho} - R${preco_pedido:.2f}")
    return preco_pedido

resultado = 0

# Enquanto verdadeiro, atribui a função realizar_pedido a var pedido, por fim a pessoa escolhe se faz um novo pedido ou nao
while True:
    pedido = realizar_pedido()
    opcao = input("Deseja pedir mais algo? (S para SIM/ N para NÃO)").strip().upper()
    resultado += pedido
    if opcao == "S":
        continue
    elif opcao == "N":
        print(resultado)
        break
    else:
        print("Opção inválida, tente novamente")
        opcao
