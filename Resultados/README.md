# Códificação das Pastas
Cenario_NomeDoJogo_RedeNeural_PoliticadeExploracao_ColetorDeDados_ReplayBuffer_Otimizador_AtualizacaoDeRede_Treinamento

Exemplo:

C1_CartPole-v1_RN-64-64_EG-345-1-0.001_CD-200-200-10_RB-100k-0.6-1.0_O-0.001_AR-0.99_T-5k-5

# Cenários de Simulação
* C1: Simulação sem critério de parada com X episódios.
* C2: Simulação com Y critério de parada com X episódios.
* C3: Simulação com critérios de parada condicionais, no qual sempre que atingir pontuação máxima, o agente é avaliado, caso apresente desempenho satisfatório(e.g 99%), encerra-se o treinamento; caso contrário volta para o loop de treinamento com avaliação recorrente.

# Controle de Versões 
| Versão | ⏳ |⏳|⏳|⏳|
|--------|-------------|-----|-----|-----|
| Episódios       | 5k | 10k | 15k | 20k          |
|V1 - DQN 🆗|                                    (Bruno)⏳| (Gabriel)🆗|(Kaio)🆗|(Nicolas)🆗|
|V2 - PER (ReplayBuffer) 🆗   |                  (Bruno)🆗| (Gabriel)🆗|(Kaio)🆗|(Nicolas)🆗|
|V2 - PER (PrioritazedReplayBuffer) 🆗   |       (Bruno)🆗| (Gabriel)🆗|(Kaio)🆗|(Nicolas)🆗|
|V2.1 - PER Priorização Média  🆗  |             (Bruno)🆗| (Gabriel)🆗|(Kaio)🆗|(Nicolas)🆗|
|V2.2 - PER Priorização Somada  🆗  |            (Bruno)🆗| (Gabriel)🆗|(Kaio)🆗|(Nicolas)🆗|
|V3 - PER Últimos Indice (Priorização 1 vez)🆗 |                      (Bruno)⏳| (Gabriel)🆗|(Kaio)⏳|(Nicolas)🆗|
|V3 - PER Últimos Indice (Priorização 2 vezes)🆗 |                      (Bruno)⏳| (Gabriel)🆗|(Kaio)⏳|(Nicolas)🆗|
|V3.1 - PER Melhores Indices (Max)  🆗  |              (Bruno)⏳| (Gabriel)🆗|(Kaio)⏳|(Nicolas)🆗|
|V3.2 - PER Melhores Indices (Semi-Trajetória 1)  🆗  |              (Bruno)⏳| (Gabriel)🆗|(Kaio)⏳|(Nicolas)🆗|
|V3.2 - PER Melhores Indices (Semi-Trajetória 2)  🆗  |              (Bruno)⏳| (Gabriel)🆗|(Kaio)⏳|(Nicolas)⏳1|
|V3.3 - PER Piores Indices (Max)  🆗  |              (Bruno)⏳| (Gabriel)🆗|(Kaio)⏳|(Nicolas)🆗|
|V3.4 - PER Piores Indices (Semi-Trajetória 1)  🆗  |              (Bruno)⏳| (Gabriel)🆗|(Kaio)⏳|(Nicolas)🆗|
|V3.4 - PER Piores Indices (Semi-Trajetória 2)  🆗  |              (Bruno)⏳| (Gabriel)🆗|(Kaio)⏳|(Nicolas)🆗|
|V4 - PER Ultima Trajetória ⏳  |                (Bruno)⏳| (Gabriel)⏳|(Kaio)⏳|(Nicolas)⏳|
|V4.1 - PER Melhores Trajetórias ⏳   |          (Bruno)⏳| (Gabriel)⏳|(Kaio)⏳|(Nicolas)⏳|
|V4.2 - PER Piores Trajetórias ⏳ |              (Bruno)⏳| (Gabriel)⏳|(Kaio)⏳|(Nicolas)⏳|

# Canvas dos Resultados
## Todos os Resultados
https://www.canva.com/design/DAGGtRS_IIk/dl3Y29Rsqo-hhn7ZD6StJA/edit?utm_content=DAGGtRS_IIk&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton
## Cenário 1
[https://www.canva.com/design/DAGGtRS_IIk/dl3Y29Rsqo-hhn7ZD6StJA/edit?utm_content=DAGGtRS_IIk&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton](https://www.canva.com/design/DAGJA15Z420/CQufhGA7qcrAZ9j9b6NG-g/edit?utm_content=DAGJA15Z420&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)
## Cenário 2
[[https://www.canva.com/design/DAGGtRS_IIk/dl3Y29Rsqo-hhn7ZD6StJA/edit?utm_content=DAGGtRS_IIk&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton](https://www.canva.com/design/DAGJA1rY6_E/K8vEPqL3kU2OjhzZSO7GRg/edit?utm_content=DAGJA1rY6_E&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)
## Cenário 3
[https://www.canva.com/design/DAGGtRS_IIk/dl3Y29Rsqo-hhn7ZD6StJA/edit?utm_content=DAGGtRS_IIk&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton](https://www.canva.com/design/DAGJA7aSFgU/iOe9vP931dhriXHqU_nEyg/edit?utm_content=DAGJA7aSFgU&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)
