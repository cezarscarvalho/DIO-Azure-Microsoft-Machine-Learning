![image](https://github.com/cezarscarvalho/DIO-Azure-Microsoft-Projetos/assets/158849910/721a73fe-865b-4416-a2cf-f5ef7a9a3eff)


# Passo a passo de um modelo de previsão e a configuração de seus pontos de extremidade:


Primeiramente você deve criar o seu espaço de trabalho (Workspace), através do [portal do Azure](https://www.portal.azure.com).

Caso, já possua um Workspace criado poderá utilizá-lo e acessar o [Launch Studio](https://ml.azure.com) 

## 💡Certifique-se de estar em seu Workspace correto

Os Passos a seguir nos permitirão criar um Modelo de Previsão com seus devidos pontos de extremidade configurados. (❁´◡`❁)

Criaremos o Aprendizado de Máquina (Machine Learning) para a previsão do aluguel de bicicletas.    
![image-1](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/05f91a3b-77e5-483e-93a7-19c85a0dc605)



# Criação de um trabalho de ML Automatizado:

No Launch Studio, nas diversas opções ao lado esquerdo selecionar  "ML AUTOMATIZADO" 

![ML Automatizado](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/1c06337e-fba4-4087-8405-51d6a02110dd)
Clique em "+ Novo trabalho de ML Automatizado"
![+ ML Automatizado](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/561be846-b229-4a83-9d4b-a1c5329cbb44)
Clique em Avançar
![Avançar ML Automatizado](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/440ff26d-0915-4f9b-93ce-1774c55144ab)
## O tipo da tarefa será Regressão (Para prever valores numéricos contínuos)
![Tipo de Dados Regressão](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/abeddb59-889d-4946-b9b5-aadd593821df)
![Criação de Dados](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/8718c095-b2d8-413b-a660-a75dbfc8a43c)
![Criar Ativo de Dados - Tipo de Dados](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/856d13f8-f542-41f3-b448-f7005bf99601)
![Arquivos Web](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/2c0f5302-1d6a-4c90-b51b-d9b51c875449)

As fontes serão fornecidas da WEB
![URL](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/86751681-ea4c-411d-9fd5-454bdfe6c7f7)
![Configurações](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/d1ca4eb5-0f9f-40d0-bc87-c8870f76cf5a)
![Path](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/d5d6faa7-c3b3-4a12-aff3-22ddafa63c5f)

Selecione "alugueldebicicletas" para continuar a enviar o ML Automatizado
![Aluguel de Bicicletas](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/a57b688e-998f-4ccb-874d-b58a5d94d85f)
![Envie ML](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/870a623d-e72b-4c6d-8b5c-b02cedf4aecc)

Expanda as Configurações Adicionais
![Config Add](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/884a258d-20fb-49bb-a1e0-bd0bfd85da89)
![Mais Configurações Add](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/0eda756f-b8c1-4901-a849-65f7e9e7621b)

Expanda a Sessão Limites

![Sessão Limites](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/ed3e8b11-b7ea-45c7-8b33-0d3ec0264260)
![Limites 2](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/173d9e40-eba1-4f9f-a495-61e34f634d56)
![Computação](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/2b954421-1550-44db-9326-823960d59f7a)

Envie o trabalho de treinamento
![Examinar](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/d6ede542-ec4b-43e8-b7eb-ea38272548d8)

A Execução demorará alguns minutos para a compilação dos dados
![Em execução](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/62336e9f-5b64-44ce-bc99-0cfba00822d5)
Ao finalizar teremos a informação de Status concluído
![Finalização](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/9a89411a-7e10-45d9-ba7b-893f76138955)
...

Pipeline com as etapas do processo e os testes realizados
![image-2](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/ba072fdc-58ac-43f5-996e-20274309c27b)
# Implementação do Modelo
![Exito no modelo](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/d3757581-6ab3-4cdc-b712-bb171b7d3268)
# Teste do Modelo

Ao lado esquerdo clique em Pontos de Extremidade, prever-alugueis, Testar
![Pontos de extremidade](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/df282152-4f27-4d2e-a8ee-2e9c0ee9c476)
![Testar](https://github.com/cezarscarvalho/Fotos-Projetos-Azure/assets/158849910/156e0fde-4b91-4d1f-9cd1-f55397989602)
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
