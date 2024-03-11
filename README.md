![Alt text](image.png)

# Passo a passo de um modelo de previsão e a configuração de seus pontos de extremidade:


Primeiramente você deve criar o seu espaço de trabalho (Workspace), através do [portal do Azure](https://www.portal.azure.com).

Caso, já possua um Workspace criado poderá utilizá-lo e acessar o [Launch Studio](https://ml.azure.com) 

## 💡Certifique-se de estar em seu Workspace correto

Os Passos a seguir nos permitirão criar um Modelo de Previsão com seus devidos pontos de extremidade configurados. (❁´◡`❁)

Criaremos o Aprendizado de Máquina (Machine Learning) para a previsão do aluguel de bicicletas.    
![Alt text](image-1.png)



# Criação de um trabalho de ML Automatizado:

No Launch Studio, nas diversas opções ao lado esquerdo selecionar  "ML AUTOMATIZADO" 

![Alt text](<ML Automatizado.png>)
Clique em "+ Novo trabalho de ML Automatizado"
![Alt text](<+ ML Automatizado.png>)
Clique em Avançar
![Alt text](<Avançar ML Automatizado.png>)
## O tipo da tarefa será Regressão (Para prever valores numéricos contínuos)
![Alt text](<Tipo de Dados Regressão.png>)
Clique em Avançar para criar o tipo de dados
![Alt text](<Criação de Dados.png>)
![Alt text](<Criar Ativo de Dados - Tipo de Dados.png>)
![Alt text](<Arquivos Web.png>)
As fontes serão fornecidas da WEB
![Alt text](URL.png)
![Alt text](Configura%C3%A7%C3%B5es.png)
![Alt text](Path.png)
Selecione "alugueldebicicletas" para continuar a enviar o ML Automatizado
![Alt text](<Aluguel de Bicicletas.png>)
![Alt text](<Envie ML.png>)
Expanda as Configurações Adicionais
![Alt text](<Config Add.png>)
![Alt text](<Mais Configurações Add.png>)
Expanda a Sessão Limites
![Alt text](<Sessão Limites.png>)
![Alt text](<Limites 1.png>)
![Alt text](<Limites 2.png>)
![Alt text](Computa%C3%A7%C3%A3o.png)
Envie o trabalho de treinamento
![Alt text](Examinar.png)
A Execução demorará alguns minutos para a compilação dos dados
![Alt text](<Em execução-1.png>)
Ao finalizar teremos a informação de Status concluído
![Alt text](Finaliza%C3%A7%C3%A3o.png)
...
Pipeline com as etapas do processo e os testes realizados
![Alt text](image-2.png)
# Implementação do Modelo
![Alt text](<Exito no modelo.png>)
# Teste do Modelo

Ao lado esquerdo clique em Pontos de Extremidade, prever-alugueis, Testar
![Alt text](<Pontos de extremidade.png>)
![Alt text](Testar.png)
...

## Para o teste foi utilizado o json abaixo:
```yaml
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
 ``````


# O Resultado foi o discriminado abaixo

![Resultado Json](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/c2daac3a-318c-4c4d-8845-33ee97243c10)

 




