class Veiculo:
    def __init__(self, marca, modelo, ano):
        self.marca = marca
        self.modelo = modelo
        self.ano = ano

# Lista para armazenar os veículos cadastrados
veiculos_cadastrados = []

def adicionar_veiculo():
    marca = input("Digite a marca do veículo: ")
    modelo = input("Digite o modelo do veículo: ")
    ano = input("Digite o ano do veículo: ")

    veiculo = Veiculo(marca, modelo, ano)
    veiculos_cadastrados.append(veiculo)
    print("Veículo cadastrado com sucesso!")

def excluir_veiculo():
    modelo = input("Digite o modelo do veículo que deseja excluir: ")

    for veiculo in veiculos_cadastrados:
        if veiculo.modelo == modelo:
            veiculos_cadastrados.remove(veiculo)
            print("Veículo removido com sucesso!")
            return

    print("Veículo não encontrado.")

def alterar_veiculo():
    modelo = input("Digite o modelo do veículo que deseja alterar: ")

    for veiculo in veiculos_cadastrados:
        if veiculo.modelo == modelo:
            marca = input("Digite a nova marca do veículo: ")
            ano = input("Digite o novo ano do veículo: ")
            veiculo.marca = marca
            veiculo.ano = ano
            print("Veículo alterado com sucesso!")
            return

    print("Veículo não encontrado.")

def listar_veiculos():
    print("Veículos cadastrados:")
    for veiculo in veiculos_cadastrados:
        print(f"Marca: {veiculo.marca}, Modelo: {veiculo.modelo}, Ano: {veiculo.ano}")

# Função principal
def main():
    while True:
        print("\nOpções:")
        print("1. Adicionar veículo")
        print("2. Excluir veículo")
        print("3. Alterar veículo")
        print("4. Listar veículos cadastrados")
        print("0. Sair")

        opcao = input("Digite o número da opção desejada: ")

        if opcao == "1":
            adicionar_veiculo()
        elif opcao == "2":
            excluir_veiculo()
        elif opcao == "3":
            alterar_veiculo()
        elif opcao == "4":
            listar_veiculos()
        elif opcao == "0":
            break
        else:
            print("Opção inválida.")

if __name__ == "__main__":
    main()v
