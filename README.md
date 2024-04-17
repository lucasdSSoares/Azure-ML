# Azure Machine Learning
## Trabalhando com Machine Learning na Prática no Azure ML

Este repositório tem como objetivo apresentar alguns laboratórios utilizando ferramentas de machine learning Azure.

Modelo de previsão de alguel de bicicletas.

Meu desafio na criação deste modelo foi prever estimativas de aluguel de bicicletas baseado em dados disponíveis na web, onde a locação de bicicletas são feitas diariamente.

- O primeiro passo a executar é mais simples, criar uma conta no portal Azure.
- Depois, para que tudo ficasse organizado criei um Resource group.
- Com o Resource group criado, através do portal IA do Azure, criei um novo trabalho de treinamento.
- Criei um modelo referenciando a tarefa executa.
- Associei o modelo ao ponto de extremidade.
- Quando a tarefa de treinamento estiver concluido temos nosso modelo e o pontos de extremidade para apresentar.

#### Input do ponto de extremidade:
~~~
 {
   "Inputs": { 
     "data": [
       {
         "day": 1,
         "mnth": 1,   
         "year": 2022,
         "season": 2,
         "holiday": 0,
         "weekday": 1,
         "workingday": 1,
         "weathersit": 2, 
         "temp": 0.3, 
         "atemp": 0.3,
         "hum": 0.3,
         "windspeed": 0.3 
       }
     ]    
   },   
   "GlobalParameters": 1.0
 }
~~~

#### Resultado 

~~~
{ 
"Results" : [ 
	0 : float 361.26578642345688                
   ]
}
~~~



