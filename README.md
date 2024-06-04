# carro
class Carro:
    def __init__(self, marca, ano, cor, modelo, velocidade=0):
        self.marca = marca
        self.ano = ano
        self.cor = cor
        self.modelo = modelo
        self.velocidade = velocidade

    def acelerar(self, aumento):
        self.velocidade += aumento
        print(f"O carro acelerou para {self.velocidade} km/h")

    def freiar(self, reducao):
        self.velocidade -= reducao
        print(f"O carro freou para {self.velocidade} km/h")

# Exemplo de uso da classe Carro
meu_carro = Carro(marca="BMW", ano=2024, cor="azul", modelo="M5", velocidade=50)
print(f"Meu carro é um {meu_carro.marca} {meu_carro.modelo} de {meu_carro.ano} e cor {meu_carro.cor}")

meu_carro.acelerar(30)
meu_carro.freiar(20)

