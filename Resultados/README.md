# Códificação das Pastas
Cenario_NomeDoJogo_RedeNeural_PoliticadeExploracao_ColetorDeDados_ReplayBuffer_Otimizador_AtualizacaoDeRede_Treinamento

Exemplo:

C1_CartPole-v1_RN-64-64_EG-345-1-0.001_CD-200-200-10_RB-100k-0.6-1.0_O-0.001_AR-0.99_T-5k-5

# Cenários de Simulação
* C1: Simulação sem critério de parada com X episódios.
* C2: Simulação com Y critério de parada com X episódios.
* C3: Simulação com critérios de parada condicionais, no qual sempre que atingir pontuação máxima, o agente é avaliado, caso apresente desempenho satisfatório(e.g 99%), encerra-se o treinamento; caso contrário volta para o loop de treinamento com avaliação recorrente.

# Controle de Versões 
| Versão | Responsável |
|--------|-------------|
|V1 - DQN |                                                                          (Bruno)|
|V2 - PER    |                                                                       (Bruno)|
|V2.1 - PER Priorização Média    |                                                                       (Bruno)|
|V3 - PER Ultimo Indice |                                                            (Nicolas)|
|V3.1 - PER Melhores Indices    |                                                      (Nicolas)|
|V3.2 - PER Piores Indices    |                                                      (Nicolas)|
|V4 - PER Ultima Trajetória   |                                                      (Gabriel)|
|V4.1 - PER Melhores Trajetórias    |                                                  (Gabriel)|
|V4.2 - PER Piores Trajetórias  |                                                      (Gabriel)|

# Canvas dos Resultados
https://www.canva.com/design/DAGGtRS_IIk/dl3Y29Rsqo-hhn7ZD6StJA/edit?utm_content=DAGGtRS_IIk&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton
