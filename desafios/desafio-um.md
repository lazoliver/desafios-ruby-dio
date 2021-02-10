# Verificar se o número é par ou impar e inteiro.

## Leia um valor inteiro *N*. Este valor será a quantidade de valores que serão lidos em seguida. Para cada valor lido, mostre uma mensagem em inglês dizendo se este valor lido é par (*EVEN*), ímpar (*ODD*), positivo (*POSITIVE*) ou negativo (*NEGATIVE*). No caso do valor ser igual a zero (0), embora a descrição zero é par, seu programa deverá imprimir apenas *NULL*.

### ENTRADA

#### A primeira linha de entrada contém um valor inteiro N(N < 10000) que indica o número de casos de teste. Cada caso de teste a seguir é um valor inteiro X (-107 <X <107)

### SAÍDA

#### Para cada caso, imprima uma mensagem correspondente, de acordo com o exemplo abaixo. Todas as letras deverão ser maiúsculas e sempre deverá haver um espaço *entre* duas palavras impressas na mesma linha.

| Input Exemple | Output Exemple |
| ------------- | -------------- |
| 4             | ODD NEGATIVE   |
| -5            | NULL           |
| 0             | ODD POSITIVE   |
| 3             | EVEN NEGATIVE  |
| -4            |                |

### RESOLUÇÃO

	ntimes = gets.strip.to_i
	out = ""
	
	ntimes.times do |num|
		num = gets.strip.to_i
	if num == 0
		out << "NULL\n"
		
	elsif num > 0 && num % 2 == 0
	out << "EVEN POSITIVE\n"
	
	elsif num > 0 && num % 2 != 0
		out << "ODD POSITIVE\n"
		
	elsif num < 0 && num % 2 == 0
		out << "EVEN NEGATIVE\n"
	
	else
		out << "ODD NEGATIVE\n"
	
	end
	end
	
	puts out
