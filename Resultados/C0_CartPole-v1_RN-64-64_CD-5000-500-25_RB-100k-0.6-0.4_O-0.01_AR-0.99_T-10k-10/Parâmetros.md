# Parâmetros
## Ambiente
env = TransformedEnv(GymEnv("CartPole-v1"), StepCounter())

## Rede Neural
value_mlp = MLP(out_features=env.action_spec.shape[-1], num_cells=[64, 64])

## Política de Exploração

## Coletor de dados
init_rand_steps = 5000

frames_per_batch = 200

optim_steps = 10

## buffer de reprodução
buffer_size = 100_000  
rb = ReplayBuffer(storage=LazyTensorStorage(buffer_size), sampler=PrioritizedSampler(max_capacity=buffer_size, alpha=0.6, beta=0.4))                    

## Módulo de perda e otimizador
optim = Adam(loss.parameters(), lr=0.02)
updater = SoftUpdate(loss, eps=0.99)

## Parâmetro de Treinamento
episodes = 20_000     
criterio_parada = NONE
