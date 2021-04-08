# Covid & Eleições-2018
Identificar possíveis comportamentos na transmissão do Covid relacionados a vieses políticos com base na eleição presidencial em 2018.

![image](https://user-images.githubusercontent.com/60569541/113933023-778f4c80-97ca-11eb-9af8-94e3e8fa0df4.png)


## **1. Motivação**
-
Vivemos um momento complicado da Covid no Brasil onde batemos recordes de óbitos diariamente. Os casos confirmados também não param de subir e, por mais que a vacinação siga firme, infelizmente um vacinado não passa anticorpos para outro indivíduo, ao contrário do vírus, que ao infectar uma pessoa continua infectando muitas outras.

Analisando os dados da Covid no Brasil, surgiu uma hipótese: Existe alguma correlação entre os casos de Covid no Brasil e as eleições presidenciais ocorridas em 2018?

Para isso, foram analisadas as seguintes bases de dados:
1. Covid: base acessada em 17/março/2021 - https://covid.saude.gov.br/
2. Resultado das eleições presidenciais 2018 (1º turno): bases por estado, acessadas através do aplicativo do TSE - https://bit.ly/3mA2bu3

Com estas bases é possível tentar responder a seguinte questão específica:
- Existe correlação entre os votos nos 3 candidatos mais votados para presidente, considerando o 1º tunro em 2018, e os casos acumulados de Covid em cada estado?

Para responder esta pergunta, é possível realizar uma análise exploratória inicial de dados.


## **2.** ***Insights***
Em resposta, podemos observar as correlações entre o % votos e no % de casos acumulados até 17/março/21 por população de cada estado:
- Mais votado: **Bolsonaro** (46.03% dos votos válidos)

    correlação = 0.55

    r²         = 0.30

- 2º mais votado: **Haddad** (29.28% dos votos válidos)
    
    correlação = -0.29
    
    r²         =  0.08

- 3º mais votado: **Ciro** (12.47% dos votos válidos)
    
    correlação = 0.04
    
    r²         = 0.0016

- Soma dos **demais candidatos** (12.22% dos votos válidos)
    
    correlação = 0.46
    
    r²         = 0.21
    





Propostas para próximos passos:
- Tipo sanguíneo
- clima 
- comparar com rejeição ao longo do tempo
- 
