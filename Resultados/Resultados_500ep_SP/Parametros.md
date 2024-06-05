# Parâmetros
num_cells=[64, 64]

annealing_num_steps=345, eps_init=1, eps_end = 0.001

lr=0.001

SoftUpdate(loss, eps=0.99)


### Linhas de Inicialização
total_count = 0     # Inicializa um contador para o número total de passos coletados.

total_episodes = 0  # Inicializa um contador para o número total de episódios completados.

episodes = 5000     # Define o número total de episódios a serem treinados.

X1 = None

score_list_1 = []

score_list_mean_100 = []

t0 = time.time()    # Armazena o tempo de início do treinamento para calcular a duração total no final.
