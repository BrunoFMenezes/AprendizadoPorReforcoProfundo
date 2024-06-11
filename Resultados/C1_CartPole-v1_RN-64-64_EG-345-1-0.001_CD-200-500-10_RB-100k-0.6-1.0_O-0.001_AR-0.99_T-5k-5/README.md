# Parâmetros
## Ambiente
env = TransformedEnv(GymEnv("CartPole-v1"), StepCounter())
## Rede Neural
value_mlp = MLP(out_features=env.action_spec.shape[-1], num_cells=[64, 64])
## Política de Exploração
exploration_module = EGreedyModule(env.action_spec, annealing_num_steps=345, eps_init=1, eps_end = 0.001)
## Coletor de dados
init_rand_steps = 200

frames_per_batch = 500

optim_steps = 10  
## Buffer de Reprodução
buffer_size = 100_000  

V1: 

rb = ReplayBuffer(storage=LazyTensorStorage(buffer_size)) 

Outras versões: 

rb = ReplayBuffer(storage=LazyTensorStorage(buffer_size), sampler=PrioritizedSampler(max_capacity=buffer_size, alpha=0.6, beta=1.0))                    
## Módulo de perda e otimizador
optim = Adam(loss.parameters(), lr=0.001)

updater = SoftUpdate(loss, eps=0.99)
## Parâmetro de Treinamento
episodes = 5000     # Define o número total de episódios a serem treinados.

criterio_parada = NONE
