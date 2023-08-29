1. Classe Bola: Crie uma classe que modele uma bola:
a. Atributos: Cor, circunferência, material
class Bola:
    def __init__(self, cor, circunferencia, material):
        self.cor = cor
        self.circunferencia = circunferencia
        self.material = material

    def mostrar_informacoes(self):
        print("Cor: ", self.cor)
        print("Circunferência: ", self.circunferencia)
        print("Material: ", self.material)
   b. Métodos: trocaCor e mostraCor
2. Classe Quadrado: Crie uma classe que modele um quadrado:
a. Atributos: Tamanho do lado
class Quadrado:
    def __init__(self, lado):
        self.lado = lado

    def trocaLado(self, novo_lado):
        self.lado = novo_lado

    def mostraLado(self):
        print("Tamanho do lado:", self.lado)
   class Quadrado:
    def __init__(self, lado):
        self.lado = lado

    def trocaLado(self, novo_lado):
        self.lado = novo_lado

    def mostraLado(self):
        print("Tamanho do lado:", self.lado)
   3. Classe Retângulo: Crie uma classe que modele um retângulo:
a. Atributos: LadoA, LadoB (ou Comprimento e Largura, ou Base e Altura,
a escolher)
class Retângulo:
    def __init__(self, base, altura):
        self.base = base
        self.altura = altura
      b. Métodos: Mudar valor dos lados, Retornar valor dos lados, calcular Área
e calcular Perímetro;
b.class Retângulo:
    def __init__(self, base, altura):
        self.base = base
        self.altura = altura

    def mudar_lados(self, nova_base, nova_altura):
        self.base = nova_base
        self.altura = nova_altura

    def retornar_lados(self):
        return self.base, self.altura

    def calcular_area(self):
        return self.base * self.altura

    def calcular_perimetro(self):
        return 2 * (self.base + self.altura)
   c. Crie um programa que utilize esta classe. Ele deve pedir ao usuário que
informe as medidas de um local. Depois, deve criar um objeto com as
medidas e calcular a quantidade de pisos e de rodapés necessárias para
o local.
# Importar a classe Retângulo
class Retângulo:
    # Implementação da classe Retângulo (incluindo atributos e métodos)

# Função principal do programa
def main():
    # Solicitar as medidas do local ao usuário
    base_local = float(input("Digite a medida da base do local em metros: "))
    altura_local = float(input("Digite a medida da altura do local em metros: "))

    # Criar um objeto Retângulo com as medidas informadas pelo usuário
    local = Retângulo(base_local, altura_local)

    # Calcular a quantidade de pisos e rodapés necessários
    area_local = local.calcular_area()
    quantidade_pisos = area_local // 0.25  # Considerando que cada piso tem 0.25 metros quadrados
    quantidade_rodapes = (2 * local.base + 2 * local.altura) // 0.10  # Considerando que cada rodapé tem 0.10 metros de comprimento

    # Exibir os resultados
    print("Quantidade de pisos necessários:", quantidade_pisos)
    print("Quantidade de rodapés necessários:", quantidade_rodapes)

# Executar o programa
main()
4. Classe Pessoa: Crie uma classe que modele uma pessoa:
class Pessoa:
    def __init__(self, nome, idade, altura):
        self.nome = nome
        self.idade = idade
        self.altura = altura

    def apresentar(self):
        print(f"Olá, meu nome é {self.nome}.")

    def envelhecer(self, anos):
        self.idade += anos

    def crescer(self, centimetros):
        self.altura += centimetros
        class Pessoa:
    def __init__(self, nome, idade, altura):
        self.nome = nome
        self.idade = idade
        self.altura = altura

    def apresentar(self):
        print(f"Olá, meu nome é {self.nome}.")

    def envelhecer(self, anos):
        self.idade += anos

    def crescer(self, centimetros):
        self.altura += centimetros
    class Pessoa:
    def __init__(self, nome, idade, altura, peso):
        self.nome = nome
        self.idade = idade
        self.altura = altura
        self.peso = peso

    def apresentar(self):
        print(f"Olá, meu nome é {self.nome}.")

    def envelhecer(self, anos):
        self.idade += anos
        if self.idade < 21:
            self.crescer(0.5 * anos)

    def engordar(self, quilos):
        self.peso += quilos

    def emagrecer(self, quilos):
        self.peso -= quilos

    def crescer(self, centimetros):
        self.altura += centimetros
        class Pessoa:
    def __init__(self, nome, idade, altura, peso):
        self.nome = nome
        self.idade = idade
        self.altura = altura
        self.peso = peso

    def apresentar(self):
        print(f"Olá, meu nome é {self.nome}.")

    def envelhecer(self, anos):
        self.idade += anos
        if self.idade < 21:
            self.crescer(0.5 * anos)

    def engordar(self, quilos):
        self.peso += quilos

    def emagrecer(self, quilos):
        self.peso -= quilos

    def crescer(self, centimetros):
        self.altura += centimetros
        class ContaCorrente:
    def __init__(self, numero_conta, nome_correntista, saldo=0):
        self.numero_conta = numero_conta
        self.nome_correntista = nome_correntista
        self.saldo = saldo

    def alterarNome(self, novo_nome):
        self.nome_correntista = novo_nome

    def deposito(self, valor):
        if valor > 0:
            self.saldo += valor
            print("Depósito realizado.")
        else:
            print("O valor do depósito deve ser maior que zero.")

    def saque(self, valor):
        if valor > 0:
            if self.saldo >= valor:
                self.saldo -= valor
                print("Saque realizado.")
            else:
                print("Saldo insuficiente.")
        else:
            print("O valor do saque deve ser maior que zero.")
            class TV:
    def __init__(self):
        self.canal = 1
        self.volume = 50

    def alterarCanal(self, novo_canal):
        if 1 <= novo_canal <= 100:
            self.canal = novo_canal
            print("Canal alterado para", novo_canal)
        else:
            print("Número de canal inválido.")

    def aumentarVolume(self):
        if self.volume < 100:
            self.volume += 1
            print("Volume aumentado:", self.volume)
        else:
            print("Volume máximo atingido.")

    def diminuirVolume(self):
        if self.volume > 0:
            self.volume -= 1
            print("Volume diminuído:", self.volume)
        else:
            print("Volume mínimo atingido.")


# Exemplo de uso da classe TV
televisor = TV()

televisor.alterarCanal(5)  # Alterando para o canal 5
televisor.aumentarVolume()  # Aumentando o volume
televisor.diminuirVolume()  # Diminuindo o volume
class BichinhoVirtual:
    def __init__(self, nome):
        self.nome = nome
        self.fome = 0
        self.saude = 100
        self.energia = 100

    def alimentar(self):
        self.fome -= 10
        self.saude += 5
        self.energia += 5
        if self.fome < 0:
            self.fome = 0
        if self.saude > 100:
            self.saude = 100
        if self.energia > 100:
            self.energia = 100
        print("Alimentando", self.nome)

    def brincar(self):
        self.fome += 5
        self.saude += 5
        self.energia -= 10
        if self.fome > 100:
            self.fome = 100
        if self.saude > 100:
            self.saude = 100
        if self.energia < 0:
            self.energia = 0
        print("Brincando com", self.nome)

    def dormir(self):
        self.fome += 10
        self.saude += 10
        self.energia = 100
        if self.fome > 100:
            self.fome = 100
        if self.saude > 100:
            self.saude = 100
        print(self.nome, "foi dormir")

    def status(self):
        print("Nome:", self.nome)
        print("Fome:", self.fome)
        print("Saúde:", self.saude)
        print("Energia:", self.energia)


# Exemplo de uso da classe BichinhoVirtual
bichinho = BichinhoVirtual("Tama")

bichinho.alimentar()  # Alimentando o bichinho
bichinho.brincar()  # Brincando com o bichinho
bichinho.dormir()  # Fazendo o bichinho dormir
bichinho.status()  # Obtendo o status do bichinho
class BichinhoVirtual:
    def __init__(self, nome):
        self.nome = nome
        self.fome = 0
        self.saude = 100
        self.idade = 0

    def alterarNome(self, novo_nome):
        self.nome = novo_nome

    def alterarFome(self, nova_fome):
        self.fome = nova_fome

    def alterarSaude(self, nova_saude):
        self.saude = nova_saude

    def alterarIdade(self, nova_idade):
        self.idade = nova_idade

    def retornarNome(self):
        return self.nome

    def retornarFome(self):
        return self.fome

    def retornarSaude(self):
        return self.saude

    def retornarIdade(self):
        return self.idade


# Exemplo de uso da classe BichinhoVirtual
bichinho = BichinhoVirtual("Tama")

bichinho.alterarNome("Novo Nome")
bichinho.alterarFome(50)
bichinho.alterarSaude(80)
bichinho.alterarIdade(5)

print("Nome:", bichinho.retornarNome())
print("Fome:", bichinho.retornarFome())
print("Saúde:", bichinho.retornarSaude())
print("Idade:", bichinho.retornarIdade())
class Macaco:
    def __init__(self, nome):
        self.nome = nome
        self.bucho = []

    def comer(self, alimento):
        self.bucho.append(alimento)

    def verBucho(self):
        print("Conteúdo do estômago de", self.nome, ":")
        for alimento in self.bucho:
            print("-", alimento)

    def digerir(self):
        self.bucho = []
        print(self.nome, "digeriu o alimento.")


# Exemplo de uso da classe Macaco
macaco1 = Macaco("Bob")
macaco2 = Macaco("Charlie")

macaco1.comer("Banana")
macaco1.comer("Maçã")
macaco1.comer("Laranja")

macaco2.comer("Amendoim")
macaco2.comer("Uva")
macaco2.comer("Pera")

macaco1.verBucho()
macaco2.verBucho()

macaco1.digerir()
macaco2.digerir()

macaco1.verBucho()
macaco2.verBucho()
class Macaco:
    def __init__(self, nome):
        self.nome = nome
        self.bucho = []

    def comer(self, alimento):
        self.bucho.append(alimento)

    def verBucho(self):
        print("Conteúdo do estômago de", self.nome, ":")
        for alimento in self.bucho:
            print("-", alimento)

    def digerir(self):
        self.bucho = []
        print(self.nome, "digeriu o alimento.")


# Exemplo de uso da classe Macaco
macaco1 = Macaco("Bob")
macaco2 = Macaco("Charlie")

macaco1.comer("Banana")
macaco1.comer("Maçã")
macaco1.comer("Laranja")

macaco2.comer("Amendoim")
macaco2.comer("Uva")
macaco2.comer("Pera")

macaco1.verBucho()
macaco2.verBucho()

macaco1.digerir()
macaco2.digerir()

macaco1.verBucho()
macaco2.verBucho(
class Ponto:
    def __init__(self, x, y):
        self.x = x
        self.y = y

class Retangulo:
    def __init__(self, ponto1, ponto2):
        self.ponto1 = ponto1
        self.ponto2 = ponto2

    def calcular_area(self):
        base = abs(self.ponto1.x - self.ponto2.x)
        altura = abs(self.ponto1.y - self.ponto2.y)
        area = base * altura
        return area

    def calcular_perimetro(self):
        base = abs(self.ponto1.x - self.ponto2.x)
        altura = abs(self.ponto1.y - self.ponto2.y)
        perimetro = 2 * (base + altura)
        return perimetro


# Função para criar pontos a partir de coordenadas
def criar_ponto(x, y):
    ponto = Ponto(x, y)
    return ponto


# Função para criar um retângulo a partir de dois pontos
def criar_retangulo(ponto1, ponto2):
    retangulo = Retangulo(ponto1, ponto2)
    return retangulo


# Programa principal
ponto1 = criar_ponto(2, 3)
ponto2 = criar_ponto(5, 7)

retangulo = criar_retangulo(ponto1, ponto2)

area = retangulo.calcular_area()
perimetro = retangulo.calcular_perimetro()

print("Área do retângulo:", area)
print("Perímetro do retângulo:", perimetro)
class Ponto:
    def __init__(self, x, y):
        self.x = x
        self.y = y
        c. Possua uma função para imprimir os valores da classe Ponto
class Retângulo:
    def __init__(self, largura, altura):
        self.largura = largura
        self.altura = altura
        def imprimir_ponto(ponto):
    print("Coordenadas do ponto: ({}, {})".format(ponto.x, ponto.y))
    def encontrar_centro_retangulo(retangulo):
    centro_x = retangulo.largura / 2
    centro_y = retangulo.altura / 2
    return Ponto(centro_x, centro_y)    
class Retângulo:
    def __init__(self, largura, altura):
        self.largura = largura
        self.altura = altura
        self.vértice_inferior_esquerdo = None

    def definir_vértice_inferior_esquerdo(self, ponto):
        self.vértice_inferior_esquerdo = ponto
        def encontrar_centro_retangulo(retangulo):
    centro_x = retangulo.vértice_inferior_esquerdo.x + retangulo.largura / 2
    centro_y = retangulo.vértice_inferior_esquerdo.y + retangulo.altura / 2
    return Ponto(centro_x, centro_y)
    def imprimir_ponto(ponto):
    print("Coordenadas do ponto: ({}, {})".format(ponto.x, ponto.y))
   def exibir_menu():
    print("--- Menu ---")
    print("1. Alterar largura do retângulo")
    print("2. Alterar altura do retângulo")
    print("3. Alterar vértice inferior esquerdo do retângulo")
    print("4. Imprimir centro do retângulo")
    print("0. Sair")
    print()

def obter_numero(opcao):
    while True:
        try:
            numero = float(input(opcao))
            return numero
        except ValueError:
            print("Valor inválido. Digite novamente.")

# Criar objeto Retângulo inicial
retangulo = Retângulo(4, 3)
vertice_inferior_esquerdo = Ponto(1, 2)
retangulo.definir_vértice_inferior_esquerdo(vertice_inferior_esquerdo)

# Loop do menu
while True:
    exibir_menu()
    opcao = input("Selecione uma opção: ")

    if opcao == "1":
        largura = obter_numero("Digite a nova largura do retângulo: ")
        retangulo.largura = largura
        print("Largura do retângulo alterada.")
    elif opcao == "2":
        altura = obter_numero("Digite a nova altura do retângulo: ")
        retangulo.altura = altura
        print("Altura do retângulo alterada.")
    elif opcao == "3":
        x = obter_numero("Digite o novo valor de x para o vértice inferior esquerdo: ")
        y = obter_numero("Digite o novo valor de y para o vértice inferior esquerdo: ")
        novo_vertice = Ponto(x, y)
        retangulo.definir_vértice_inferior_esquerdo(novo_vertice)
        print("Vértice inferior esquerdo do retângulo alterado.")
    elif opcao == "4":
        centro = encontrar_centro_retangulo(retangulo)
        imprimir_ponto(centro)
    elif opcao == "0":
        print("Encerrando o programa...")
        break
    else:
        print("Opção inválida. Digite novamente.")
        class BombaDeCombustivel:
    def __init__(self, tipo_combustivel, valor_litro, quantidade_combustivel):
        self.tipo_combustivel = tipo_combustivel
        self.valor_litro = valor_litro
        self.quantidade_combustivel = quantidade_combustivel

    def abastecer_por_valor(self, valor):
        litros_abastecidos = valor / self.valor_litro
        if litros_abastecidos <= self.quantidade_combustivel:
            self.quantidade_combustivel -= litros_abastecidos
            return litros_abastecidos
        else:
            litros_possiveis = self.quantidade_combustivel
            self.quantidade_combustivel = 0
            return litros_possiveis

    def abastecer_por_litro(self, litros):
        valor_pagar = litros * self.valor_litro
        if litros <= self.quantidade_combustivel:
            self.quantidade_combustivel -= litros
            return valor_pagar
        else:
            litros_possiveis = self.quantidade_combustivel
            valor_pagar = litros_possiveis * self.valor_litro
            self.quantidade_combustivel = 0
            return valor_pagar

    def alterar_valor_litro(self, novo_valor):
        self.valor_litro = novo_valor

    def alterar_tipo_combustivel(self, novo_tipo):
        self.tipo_combustivel = novo_tipo

    def alterar_quantidade_combustivel(self, nova_quantidade):
        self.quantidade_combustivel = nova_quantidade

    def exibir_status(self):
        print("Tipo de Combustível:", self.tipo_combustivel)
        print("Valor por Litro: R$", self.valor_litro)
        print("Quantidade de Combustível: %.2f litros" % self.quantidade_combustivel)


# Programa principal
bomba = BombaDeCombustivel("Gasolina", 5.0, 100.0)

print("Bem-vindo à Bomba de Combustível!")
print()
print("Opções:")
print("1. Abastecer por Valor")
print("2. Abastecer por Litro")
print("3. Alterar Valor por Litro")
print("4. Alterar Tipo de Combustível")
print("5. Alterar Quantidade de Combustível")
print("6. Exibir Status")
print("0. Sair")
print()

while True:
    opcao = input("Selecione uma opção: ")

    if opcao == "1":
        valor = float(input("Digite o valor em reais para abastecer: "))
        litros_abastecidos = bomba.abastecer_por_valor(valor)
        print("Abastecimento realizado. Litros abastecidos:", litros_abastecidos)
    elif opcao == "2":
        litros = float(input("Digite a quantidade de litros para abastecer: "))
        valor_pagar = bomba.abastecer_por_litro(litros)
        print("Abastecimento realizado. Valor a pagar: R$", valor_pagar)
    elif opcao == "3":
        novo_valor = float(input("Digite o novo valor por litro: "))
        bomba.alterar_valor_litro(novo_valor)
        print("Valor por litro alterado.")
    elif opcao == "4":
        novo_tipo = input("Digite o novo tipo de combustível: ")
        bomba.alterar_tipo_combustivel(novo_tipo)
        print("Tipo de combustível alterado.")
    elif opcao == "5":
        nova_quantidade = float(input("Digite a nova quantidade de combustível: "))
        bomba.alterar_quantidade_combustivel(nova_quantidade)
        print("Quantidade de combustível alterada.")
    elif opcao == "6":
        bomba.exibir_status()
    elif opcao == "0":
        print("Encerrando o programa...")
        break
    else:
        print("Opção inválida. Digite novamente.")
        class BombaDeCombustivel:
    def __init__(self, tipo_combustivel, valor_litro, quantidade_combustivel):
        self.tipo_combustivel = tipo_combustivel
        self.valor_litro = valor_litro
        self.quantidade_combustivel = quantidade_combustivel
        class BombaDeCombustivel:
    def __init__(self, tipoCombustivel, valorLitro, quantidadeCombustivel):
        self.tipoCombustivel = tipoCombustivel
        self.valorLitro = valorLitro
        self.quantidadeCombustivel = quantidadeCombustivel
        class BombaDeCombustivel:
    def __init__(self, tipoCombustivel, valorLitro, quantidadeCombustivel):
        self.tipoCombustivel = tipoCombustivel
        self.valorLitro = valorLitro
        self.quantidadeCombustivel = quantidadeCombustivel

    def abastecerPorValor(self, valor):
        litros_abastecidos = valor / self.valorLitro
        self.quantidadeCombustivel -= litros_abastecidos
        return litros_abastecidos
        ii. abastecerPorLitro( ) – método onde é informado a quantidade em
litros de combustível e mostra o valor a ser pago pelo cliente.
class BombaDeCombustivel:
    def __init__(self, tipoCombustivel, valorLitro, quantidadeCombustivel):
        self.tipoCombustivel = tipoCombustivel
        self.valorLitro = valorLitro
        self.quantidadeCombustivel = quantidadeCombustivel

    def abastecerPorLitro(self, litros):
        valor_pagar = litros * self.valorLitro
        self.quantidadeCombustivel -= litros
        return valor_pagar
        class BombaDeCombustivel:
    def __init__(self, tipoCombustivel, valorLitro, quantidadeCombustivel):
        self.tipoCombustivel = tipoCombustivel
        self.valorLitro = valorLitro
        self.quantidadeCombustivel = quantidadeCombustivel

    def alterarValor(self, novo_valor):
        self.valorLitro = novo_valor
        iv. alterarCombustivel( ) – altera o tipo do combustível.
v. alterarQuantidadeCombustivel( ) – altera a quantidade de
combustível restante na bomba.
class BombaDeCombustivel:
    def __init__(self, tipoCombustivel, valorLitro, quantidadeCombustivel):
        self.tipoCombustivel = tipoCombustivel
        self.valorLitro = valorLitro
        self.quantidadeCombustivel = quantidadeCombustivel

    def alterarQuantidadeCombustivel(self, nova_quantidade):
        self.quantidadeCombustivel = nova_quantidade
        
