## Você terá o desafio de ler um valor inteiro correspondente à identidade de uma pessoa em dias e informe-a em anos, meses e dias.

### Obs.: Apenas para facilitar o cálculo, considere todo ano com 365 dias e todo mês com 30 dias. Nos casos de teste nunca haverá uma situação que permite 12 meses e alguns dias, como 360, 363 ou 364.

### ENTRADA

#### O arquivo de entrada contém um valor inteiro.

#### SAÍDA

#### Imprima a saída conforme exemplo fornecido.

| Input Exemple | Output Exemple                         |
| ------------- | -------------------------------------- |
| 400           | 1 ano(s)<br />1 mes(es)<br />5 dias(s) |

| Input Exemple | Output Exemple                              |
| ------------- | ------------------------------------------- |
| 800           | 2 ano(s)<br />2 mes(es)<br />10 dias(s)**** |

| Input Exemple | Output Exemple                         |
| ------------- | -------------------------------------- |
| 30            | 0 ano(s)<br />1 mes(es)<br />0 dias(s) |

### RESOLUÇÃO

	idade_dias = gets.strip.to_i
	
	idade_anos = idade_dias / 365;
	idade_meses = ((idade_dias % 365) / 30);
	idade_dias = ((idade_dias % 365) % 30);
	
	puts "#{idade_anos} ano(s)"
	puts "#{idade_meses} mes(es)"
	puts "#{idade_dias} dia(s)"

