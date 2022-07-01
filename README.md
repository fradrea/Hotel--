programa 
{
	funcao inicio() 
	{
	    real diaria, totalDias = 0.0 
	    cadeia nome, sinal     = "continua"
	    inteiro idade          = 0, gratuito = 0, meia = 0
	    
	    
	    escreva("qual o valor da diária, \n")
	    leia(diaria)
	    
	    enquanto(sinal!= "s" e sinal!= "n")
	    {
	    escreva("qual o nome do hospede,\n")
	    leia(nome)
	    escreva("qual a idade maior ou idade menor,\n")
	    leia(idade)
	    escreva("para continuar registrando hospede digite continua,ex:[s] ou [n],\n")
	    se(idade<4)
	    {
	        escreva(nome,"possui gratuidade,\n")
	        gratuito++
	        escreva("para continuar registrando hospede digite continua,ex:[s] ou [n],\n")
	        leia(sinal)
	        limpa()
	    }
	    senao se(idade>80)
	    {
	        totalDias=totalDias+0.5*diaria
	        escreva(nome,"paga meia,\n")
	        meia++
	        escreva("para continuar registrando hospede digite continuar,ex:[s] ou [n] ,\n")
	        leia(sinal)
	        limpa()
	   }
	   
	   
	    }
	    escreva("o total de hospedagem é:R$",totalDias,";",gratuito,"gratuidade(s);",meia,"meia(s)")
	    
		
	}
}
