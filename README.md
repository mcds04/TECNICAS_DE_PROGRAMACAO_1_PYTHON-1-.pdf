# TECNICAS_DE_PROGRAMACAO_1_PYTHON-1-.pdf
ESTRUTURA DE REPETIÇÃO EM LINGUAGEM PYTHON
DISCIPLINA: TÉCNICAS DE PROGRAMAÇÃO I  
DOCENTE: EDVAR DA LUZ OLIVEIRA  
DISCENTE: MARIA CRISTINA SOUSA 
ASSUNTO: ESTRUTURA DE REPETIÇÃO EM LINGUAGEM PYTHON  
  
LISTA DE EXERCÍCIOS   
  
1. Desenvolva um programa que execute as 5 primeiras tabuadas (tabuada do 1, 2, 3, 4 e 5). Utilize o laço de repetição while ().  
Resposta:  
for i in range (1, 11):     print(f'{i}x{i}={i*i}') 
 
 
 
Saida:  
1x1=1 
2x2=4 
3x3=9 
4x4=16 
5x5=25 
6x6=36 
7x7=49 
8x8=64 
9x9=81 
10x10=100 
2. Desenvolva um programa que imprima na tela a tabuada de um valor determinado pelo usuário. Utilize o laço de repetição for ().  
Resposta: num = int (input("Digite um número: ")) 
for i in range (1, 11):     print(f'{num} x {i} = {num*i}') 
 
Saída: Digite um número: 6 
6 x 1 = 6 
6 x 2 = 12 
6 x 3 = 18 
 
6 x 4 = 24 
6 x 5 = 30 
6 x 6 = 36 
6 x 7 = 42 
6 x 8 = 48 
6 	x 9 = 54 
6 x 10 = 60 
 
• Desenvolva um programa de apresente um menu com as opções Clientes,  Fornecedores, Encomendas e Sair. Utilize o laço de repetição while ().  
Resposta: while True: 
    print ("MENU PRINCIPAL\n\nC-Clientes\n\nF-Fornecedores\n\nEEncomendas\n\nS-Sair")     opcao = input (">Escolha uma opção: ")     if opcao. Upper () == 'C':         print ("Opção CLIENTES")     elif opcao. Upper () == 'F': 
        print ("Opção FORNECEDORES")     elif opcao. Upper () == 'E':         print ("Opção ENCOMENDAS")     elif opcao. Upper () == 'S':         print ("Finalizando...")         break     else: 
        print ("Opção inválida. Tente novamente.") 
 
 
Saída:  
MENU PRINCIPAL 
 
C-Clientes 
 
F-Fornecedores 
 
E-Encomendas 
 
S-Sair 
>Escolha uma opção: c 
Opção CLIENTES 
MENU PRINCIPAL 
 
C-Clientes 
 
F-Fornecedores 
 
E-Encomendas 
 
S-Sair 
>Escolha uma opção: F 
Opção FORNECEDORES 
MENU PRINCIPAL 
 
C-Clientes 
 
F-Fornecedores 
 
E-Encomendas 
 
S-Sair 
>Escolha uma opção: S Finalizando... 
3. Desenvolva um programa que calcule a soma entre todos os números ímpares que são múltiplos de 3 e que se encontram no intervalo de 1 até 500. Utilize o laço de repetição for ().  
Resposta:  
soma = 0 for i in range (1, 500, 2):     if i % 3 == 0:         soma += i print (f"A soma dos números ímpares múltiplos de 3 no intervalo de 
1 a 500 é {soma}.") 
 
 
Saída: A soma dos números ímpares múltiplos de 3 no intervalo de 1 a 500 é 20667 
Utilizando o laço de repetição while ()while, desenvolva um programa que crie uma matriz 4x4 idêntico ao exemplo abaixo:  
 	𝟏 	𝟐 	𝟑  	 𝟒 
 	𝟐 	𝟒 	𝟔    𝟖 
 	[ 	]  
 	𝟑 	𝟔  𝟗  𝟏𝟐 
 	  𝟒 	𝟖 	𝟏𝟐   𝟏𝟔   
Resposta:  
i	= 1 while i <= 4: 
j	= 1     while j <= 4: 
        print (i * j, end =' ')         j += 1     print ()     i += 1  
 
 
Saída:  
1	2 3 4  
2	4 6 8  
3	6 9 12  
4	8 12 16 
4.	Desenvolva um programa que leia um número inteiro e diga se ele é ou não um NÚMERO PRIMO. Utilize a estrutura de repetição que melhor se enquadra para esse problema.   
5.	def È_primo(número): 
6.	if número < 2: 
7.	return false 
8.	for i in range (2, número): 
9.	if número % i == 0: 
10.	return false 
11.	return True 
12.  
13.	numeros = [18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30,] 
14.	for número in numeros: 
15.	if È_primo(número): 
16.	print(f"{número} é PRIMO.") 
17.	else: 
18.	print(f"{número} NÃO É PRIMO.") 
 
 
Saída:  
18 NÃO É PRIMO. 19 É PRIMO. 
20	NÃO É PRIMO. 
21	NÃO É PRIMO. 
22	NÃO É PRIMO. 23 É PRIMO. 
24	NÃO É PRIMO. 
25	NÃO É PRIMO. 
26	NÃO É PRIMO. 
27	NÃO É PRIMO. 
28	NÃO É PRIMO. 
29	É PRIMO. 
30	NÃO É PRIMO. 
19. Crie um programa que leia vários números inteiros, o programa deve possuir como critério de parada o valor 999 que será digitado pelo usuário. No final, mostre quantos números foram digitados e qual foi a soma entre eles (a soma deve desconsiderar o 999). Utilize o laço de repetição while ().  
Resposta:  
soma = 0 quantidade = 0 número = int(input("Digite um número inteiro: ")) while número! = 999:     soma += número     quantidade += 1     número = int (input("Digite um número inteiro: ")) print (f"O valor {quantidade} das somas entre eles é {soma}.") 
 
Saída:  
Digite um número inteiro: 20 
Digite um número inteiro: 200 
Digite um número inteiro: 350 
Digite um número inteiro: 999 
O valor 3 das somas entre eles é 570. 
20. Crie um programa que leia dois valores e mostre um menu conforme tabela abaixo. O programa deverá realizar a operação solicitada em cada caso. Utilize o laço de repetição while ().  
Código  	Operação  
[1]  	Somar  
[2]  	Multiplicar  
[3]  	Maior  
[4]  	Novos números  
[5]  	Sair do Programa  
  
Resposta:  
valor1 = int (input("Digite o primeiro valor: ")) valor2 = int (input("Digite o segundo valor: ")) opcao = 0 while opcao! = 5: 
    print ("Código Operação")     print ("[1] Somar")     print ("[2] Multiplicar")     print ("[3] Maior")     print ("[4] Novos números")     print ("[5] Sair do Programa") 
    opcao = int (input ("Qual a sua opção? "))     if opcao == 1:         print (f"A soma entre {valor1} e {valor2} é 
{valor1+valor2}.")     elif opcao == 2:         print (f"O produto entre {valor1} e {valor2} é 
{valor1*valor2}.")     elif opcao == 3: 
        if valor1 > valor2: 
            print(f"{valor1} é maior que {valor2}.")         elif valor2 > valor1: 
            print(f"{valor2} é maior que {valor1}.") 
        else: 
            print ("Os valores são iguais.")     elif opcao == 4: 
        valor1 = int (input ("Digite o primeiro valor: "))         valor2 = int (input ("Digite o segundo valor: ")) print ("Finalizando...") 
 
 
Saída:  
Digite o primeiro valor: 1 
Digite o segundo valor: 2 
Código Operação [1] Somar 
[2]	Multiplicar 
[3]	Maior 
[4]	Novos números 
[5]	Sair do Programa Qual a sua opção? 3 
2 é maior que 1. 
Código Operação [1] Somar 
[2]	Multiplicar 
[3]	Maior 
[4]	Novos números 
[5]	Sair do Programa 
Qual a sua opção? 4 
Digite o primeiro valor: 5 
Digite o segundo valor: 2 
Código Operação [1] Somar 
[2]	Multiplicar 
[3]	Maior 
[4]	Novos números 
[5]	Sair do Programa Qual a sua opção? 5 
Finalizando... 
21. Faça um programa que leia o peso em kg de 5 pessoas. No final, mostre qual foi o maior e o menor peso lidos. Utilize o laço de repetição for ().  
Resposta:  
maior = menor = float (input ("Peso da 1ª pessoa: "))  
for i in range (2, 6): 
    peso = float (input (f"Peso da {i}ª pessoa: "))      if peso > maior:         maior = peso      if peso < menor:         menor = peso  
print (f'O maior peso lido foi de {maior}kg e o menor foi de 
{menor}kg.')  
 
Saída:  
Peso da 1ª pessoa: 50 
Peso da 2ª pessoa: 60 
Peso da 3ª pessoa: 70 
Peso da 4ª pessoa: 80 
Peso da 5ª pessoa: 108 
O maior peso lido foi de 108.0kg e o menor foi de 50.0kg. 
22. Desenvolva um programa que gere 20 números aleatórios determinados em um intervalo de 1 a 500. Utilize o laço de repetição for ().  
 
Respostas:  
import random  for _ in range(20):  
    print(random.randint(1, 500))  
 
Saída:  
21 
229 
200 
483 44 
351 
147 
112 
433 
385 
153 
188 
292 
271 
329 
369 
371 
123 
327 
423 
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
ANEXO (QUESTÃO 1) 
   
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
 
   
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
   
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
   
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
 
ANEXO (QUESTÃO 5)  
   
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
ANEXO (QUESTÃO 6)  
   
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
ANEXO (QUESTÃO 7)  
   
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
ANEXO (QUESTÃO 8)  
   
  
   
  
 
  
  
ANEXO (QUESTÃO 9)  
   
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
 
 
ANEXO (QUESTÃO 10) – RESOLUÇÃO DE EXERCÍCIO  
   
  
  
  
  
  

