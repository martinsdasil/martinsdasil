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
