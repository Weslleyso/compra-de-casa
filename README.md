# compra-de-casa
#Programa que lê o o valor da casa que a pessoa deseja comprar, seu salário e em quantos anos deseja pagar. não podendo exceder 30% do seu salário em suas prestações.

valor = int(input('qual valor da casa?: '))
salario = int(input('qual seu salário?: '))
anos = int(input('quantos anos você ira pagar?: '))

prestação = valor/12 
prestaçãoano = prestação/anos 
limite = (salario)*30/100

if prestaçãoano > limite:
    print('não pode fazer a compra, pois sua prestação excede o limte de 30% do seu salario  ')

else:
    print(f'poderá fazer a compra em {anos} anos com uma prestaçaõ de {prestaçãoano:7.2f} reais')
