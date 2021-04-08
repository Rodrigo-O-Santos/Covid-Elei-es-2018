# Covid & Eleições-2018
Identificar possíveis comportamentos na transmissão do Covid relacionados a vieses políticos com base na eleição presidencial em 2018.

![image](https://user-images.githubusercontent.com/60569541/113933023-778f4c80-97ca-11eb-9af8-94e3e8fa0df4.png)



## **1. Motivação**
Vivemos um momento complicado da Covid no Brasil onde batemos recordes de óbitos diariamente. Os casos confirmados também não param de subir e, por mais que a vacinação siga firme, infelizmente um vacinado não passa anticorpos para outro indivíduo, ao contrário do vírus, que ao infectar uma pessoa continua infectando muitas outras.

Analisando os dados da Covid no Brasil, surgiu uma hipótese: Existe alguma correlação entre os casos de Covid no Brasil e as eleições presidenciais ocorridas em 2018?

Para isso, foram analisadas as seguintes bases de dados:
1. Covid: base acessada em 17/março/2021 - https://covid.saude.gov.br/
2. Resultado das eleições presidenciais 2018 (1º turno): bases por estado, acessadas através do aplicativo do TSE - https://bit.ly/3mA2bu3

Com estas bases é possível tentar responder a seguinte questão específica:
- Existe correlação entre os votos nos 3 candidatos mais votados para presidente, considerando o 1º tunro em 2018, e os casos acumulados de Covid em cada estado?

Para responder esta pergunta, é possível realizar uma análise exploratória inicial de dados.


## **2. Resultados das análises**
Podemos observar que as correlações entre o % votos e no % de casos acumulados até 17/março/21 por população de cada estado variam de acordo com o candidato analisado:
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


## **3. Principal argumento**
"As evidências disponíveis atualmente apontam que o vírus causador da COVID-19 pode se espalhar por meio do contato direto, indireto (através de superfícies ou objetos contaminados) ou próximo (na faixa de um metro) com pessoas infectadas através de secreções como saliva e secreções respiratórias ou de suas gotículas respiratórias, que são expelidas quando uma pessoa tosse, espirra, fala ou canta. As pessoas que estão em contato próximo (a menos de 1 metro) com uma pessoa infectada podem pegar a COVID-19 quando essas gotículas infecciosas entrarem na sua boca, nariz ou olhos." ***Organização Pan-Americana da Saúde (OPAS)***

Com isso, é esperado que os indivíduos mantenham boa higiene das mãos, usem máscara de proteção facial e distanciamento social para evitar o contágio. Porém, algumas pessoas não acreditam ou não seguem estas orientações que tem a sua origem na OMS - Organização Mundial da Saúde.

No Brasil, este tema se politizou através de comportamentos e discursos do Presidente da República ao não seguir as recomendações da OMS enquanto adversários políticos adotavam medidas opostas, seguindo todas as recomendações.

A hipótese anteriormente apresentada neste artigo, tem como argumento a conduta dos eleitores que, seguindo o comportamento dos seus respectivos candidatos, poderiam ou não, contribuir com uma maior transmissão do vírus.

Para contextualizar, podemos ver estados do país onde houve predominância dos votos em determinados candidatos nas eleições de 2018:
   
   - **SC** com **65%** dos votos válidos em **Bolsonaro**;
     
   - **PI** com **63%** dos votos válidos em **Haddad**;
    
   - **CE** com **40%** dos votos válidos em **Ciro**.

Neste sentido, se os eleitores do Bolsonaro seguem o comportamento do Presidente, então não se preocupariam com a higiene das mãos, não usariam máscaras de proteção facial e não evitariam aglomerações. Como consequência, haveria maior casos de Covid/população (%) em locais de predominância dos votos no Presidente.


## **4. Etapas do projeto**
O projeto teve os seguintes passos:

**Passo 1 -** Descrição dos dados
Identificação de dados ausentes, tipos de dados e alterações relevantes para futura análise.

**Passo 2 -** Inclusão de variáveis
Inclusão de novas variáveis para permitir maior e mais completa análise através de dados relevantes adicionados ao *dataset*.

**Passo 3 -** Análise dos dados
Verificação de correlações entre as variáveis descritas anteriormente usando análise bivariada e multivariada.



## **5. Principais *insights***
   1. Voto em Bolsonaro, é o que possui a maior correlação positiva em relação aos casos acumulados de Covid por população por estado. Analisando cada estado, quanto maior o percentual de votos em Bolsonaro, maior o percentual de número de casos de Covid por população.
   2. Os estados do PI (63% de votos em Haddad e 11% em Ciro) e CE (40% de votos em Ciro e 33% em Haddad) foram os que menos votaram em Bolsonaro (% de votos/população) e figuram entre os que possuem menor taxa percentual de casos de Covid pela população.
   3. Os estados do RJ e SP, apesar de terem mais de 50% de votos no Bolsonaro, estão entre os 11 estados com menor % de casos acumulados de Covid em relação à população, assim como PI e CE.



## **6. Conclusões**
O coeficiente de correlação se mostra efetivo para medir o grau de correlação, assim como a sua direção (positiva ou negativa) entre duas variáveis de escala métrica. 

Variando entre -1 e 1 onde:

- correlação = 0, indica que as variáveis não dependem uma da outra.

- correlação 1, indica uma correlação positiva perfeita entre as variáveis.

- correlação -1, indica uma correlação negativa perfeita (se uma aumenta, a outra diminui).

Importante estar atento à correta interpretação do coeficiente:

0.9 para mais ou para menos indica uma correlação muito forte.
0.7 a 0.9 positivo ou negativo indica uma correlação forte.
0.5 a 0.7 positivo ou negativo indica uma correlação moderada.
0.3 a 0.5 positivo ou negativo indica uma correlação fraca.
0 a 0.3 positivo ou negativo indica uma correlação desprezível.

Apesar da existência de uma correlação moderada entre duas variáveis nesta pesquisa, é importante entender como elas se correlacionam com todo o contexto, para não incorrer no erro de chegarmos a uma conclusão baseada em uma mera eventualidade. 


## **7. Próximos passos**
Espera-se o aprimoramento desta pesquisa tornando-a mais robusta através da inclusão de novas variáveis relevantes ao *dataset*. Algumas sugestões para novos ciclos do CRISP:
- Inclusão da condição geral de saúde das pessoas infectadas como o tipo sanguíneo;
- O clima e a taxa de infecção pelo Covid por estação em cada estado;
- Comparar a taxa de infecção pelo Covid em cada estado, de acordo com o aumento da rejeição do Presidente.
