![image](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/721a73fe-865b-4416-a2cf-f5ef7a9a3eff)


# Passo a passo de um modelo de previsão e a configuração de seus pontos de extremidade:


Primeiramente você deve criar o seu espaço de trabalho (Workspace), através do [portal do Azure](https://www.portal.azure.com).

Caso, já possua um Workspace criado poderá utilizá-lo e acessar o [Launch Studio](https://ml.azure.com) 

## 💡Certifique-se de estar em seu Workspace correto

Os Passos a seguir nos permitirão criar um Modelo de Previsão com seus devidos pontos de extremidade configurados. (❁´◡`❁)

Criaremos o Aprendizado de Máquina (Machine Learning) para a previsão do aluguel de bicicletas.    
![image-1](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/412fafe9-9dc4-4e63-ab87-88ba72620ffc)



# Criação de um trabalho de ML Automatizado:

No Launch Studio, nas diversas opções ao lado esquerdo selecionar  "ML AUTOMATIZADO" 

![ML Automatizado](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/a9e60236-0cbb-4cdd-b5d1-da1da14cdc4a)
Clique em "+ Novo trabalho de ML Automatizado"
![+ ML Automatizado](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/a88ca61c-dc2e-49f8-9cbe-d47a14c5788f)
Clique em Avançar
![Avançar ML Automatizado](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/c40f590c-b448-4bb2-b483-b02fba23b8f3)
## O tipo da tarefa será Regressão (Para prever valores numéricos contínuos)
![Tipo de Dados Regressão](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/a79302be-76c5-4f78-8479-a34a02e2d934)
![Criação de Dados](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/52d1ef05-bf1b-4432-95fd-abbd28ab986b)
![Criar Ativo de Dados - Tipo de Dados](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/585043ac-4994-4928-9ab9-72633a5a9e49)
![Arquivos Web](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/add29ab6-83f1-4edb-ae7d-57a54087283b)

As fontes serão fornecidas da WEB
![URL](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/d35faf4d-e650-4065-8f10-6734fabf7cbe)


![Configurações](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/a97e49a3-42d8-41b3-b97e-72d4a384a235)
![Path](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/b2279cb5-feba-45fa-981f-3b4922700599)

Selecione "alugueldebicicletas" para continuar a enviar o ML Automatizado
![Aluguel de Bicicletas](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/b9364601-526e-482e-bc0a-ccda737121d7)
![Envie ML](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/0389d91b-4ded-4510-864a-f070fb085b2d)

Expanda as Configurações Adicionais
![Config Add](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/670b4a47-717c-4575-90a4-8b2b1c236ddd)
![Mais Configurações Add](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/f41f34a2-aea2-46e3-ab6e-b78e21e05f4a)


Expanda a Sessão Limites

![Sessão Limites](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/9bde8738-9b66-45e8-9c66-36410cd7cd84)
![Limites 2](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/b6f57fb9-7b8b-4954-be40-5d45ceb384f1)
![Computação](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/2dda7352-c34e-4423-93e7-7c149e0db3f6)


Envie o trabalho de treinamento
![Examinar](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/06e1ac29-b200-4f9b-933c-10738db325d8)

A Execução demorará alguns minutos para a compilação dos dados
![Em execução-1](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/a907a74a-9192-4b4a-841c-b024e21b940e)
Ao finalizar teremos a informação de Status concluído
![Finalização](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/60f6cc01-dc55-4a29-8709-cb9e454d113d)
...

Pipeline com as etapas do processo e os testes realizados
![image-2](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/226dc15b-90be-41a8-a485-71b27c4f0dad)
# Implementação do Modelo
![Exito no modelo](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/e2099a98-2040-4624-9a81-b6dd5f76d335)
# Teste do Modelo

Ao lado esquerdo clique em Pontos de Extremidade, prever-alugueis
![Pontos de extremidade](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/7b7bc0c3-ee54-4d73-a0ef-3eefabc51181)
Testar
![Testar](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/939625ae-208e-4166-8bd2-fa29a14d91fc)
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

![Resultado Json](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/2ba97c97-f855-48d3-b4fa-e267f31700e1)
