# jogochute
 Jogo de adivinhar números

programa
{
	funcao inicio()
	{
	inteiro num, chute, tent
		escreva (">>>> Jogo do chute - Adivinhar qual o número que seu oponente digitou <<<<")		//cabeçalho
	escreva ("\n\nSem outra pessoa ver, digite o número de 0 a 9 e tecle enter: ")					//numero a ser advinhado
	leia (num)
	limpa()
	escreva (">>>> Jogo do chute - Adivinhar qual o número que seu oponente digitou <<<<")			//cabeçalho
	chute=-1
	tent=1
		
		enquanto (tent<=5 e num!=chute) {
		escreva ("\n\nChute o número digitado: ")											//tentativa adivinhacao
		leia (chute)
		se (num>chute) {
		escreva ("O número é maior do que "+chute)											//menor que o numero
		escreva ("\nTentativa "+tent+" de 5")
		}
		se (num<chute) {
		escreva ("O número é menor do que "+chute)											//maior que o numero
		escreva ("\nTentativa "+tent+" de 5")
		}
		tent=tent+1
		}
		se (num==chute) {
		escreva ("\nVocê acertou em "+(tent-1)+" tentativas!!")										//quando acertar
		escreva ("\n>>>> "+num+" é o número correto <<<<")
		escreva ("\n        ___________")
      	escreva ("\n       |           |--.")
      	escreva ("\n       |     "+(tent-1)+"º    |  |")
      	escreva ("\n       |   LUGAR!  |  |")
      	escreva ("\n        |         |---'")
      	escreva ("\n         |       |")
      	escreva ("\n          |     |")
      	escreva ("\n         __|   |__")
      	escreva ("\n        '---------'\n\n")
		}
      	senao se (tent>5) {
      	escreva ("\n\n\nVocê não acertou em "+(tent-1)+" tentativas, VOCÊ PERDEU...\n\n")
      	}
		}
}

