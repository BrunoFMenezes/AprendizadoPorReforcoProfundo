# Aprendizado Por Reforço Profundo
## Ebook DQN usando TorchRL
[Clique aqui para ir para o diretório do Ebook 📚](https://github.com/BrunoFMenezes/prompts-recipe-to-create-a-ebook/tree/main)
## Classes de ReplayBuffer da TorchRL
https://github.com/pytorch/rl/blob/main/torchrl/data/replay_buffers/replay_buffers.py#L901
## Classes de Samplers da TorchRL
https://github.com/pytorch/rl/blob/main/torchrl/data/replay_buffers/samplers.py
### Tutorial Prioritazy
https://pytorch.org/rl/stable/reference/generated/torchrl.data.replay_buffers.PrioritizedSampler.html?highlight=prioritizedsampler#torchrl.data.replay_buffers.PrioritizedSampler
## Ideias de Novas Versões
1. PER Buffer Duplo: começa usando um buffer e gera outro buffer com as melhores/piores trajetórias(experiências), após 50% do treinamento migra para o outro buffer e continua armanzenando nos dois buffer, um com as trajetórias normais e outro só com as melhores/piores trajetórias.
2. [ COMPLETE A LISTA]
