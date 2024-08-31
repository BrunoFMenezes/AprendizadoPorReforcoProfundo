# TRABALHOS FUTUROS
## Orientação de Apresentação de Solução:
1. Criar um arquivo do tipo *.ipynb*  na pasta *Soluções* dentro desse diretório;
2. Usar a seguinte codificação para o nome do arquivo:

   MS_X (Item X da lista de Melhoria de Simulação) ou NV_X (Item X da lista de Novas Versões);
## Melhorias para as Simulações - MS
1. Nas próximas simulações, adotar a relação 80-20 (Pareto). Pontuação acima de 80% é boa e abaixo de 20% é ruim. Atualmente, usa-se 60-10, mas deveria ser proporcional e complementar, ou seja, 90-10, para evitar muitas "classes".
2. Colocar tempos em minutos
3. Corrigir cálculo da taxa de sucesso
4. Corrigir exibição de log para exibir a cada 500 episódios sempre
5. Codificar a data para incluir na planila como data e hora da simulação
## Ideias de Novas Versões - NV
1. PER Buffer Duplo: começa usando um buffer e gera outro buffer com as melhores/piores trajetórias(experiências), após 50% do treinamento migra para o outro buffer e continua armanzenando nos dois buffer, um com as trajetórias normais e outro só com as melhores/piores trajetórias.
2. Compartilhamento de aprendizado. Ambiente multi agente compartilhando informações para evoluir mais rápido. Esse princípio pode ser aplicado a carros autônomos ou aplicativos de geração de rotas como o Goggle Maps e Waze.
3. Bias Correction para corrigir ainda mais a superestimação de valores Q. Uso de amostragem uniforme com probabilidade compensada.
4. Exploração baseada em incertezas;
5. Regularização L2 ou a técnica de dropout: para melhorar a generalização da rede.
6. Técnicas de compressão de modelos ou quantização de pesos: para reduzir o tamanho do modelo e o custo computacional.
7. Técnicas de paralelizaçao e distribuição: para aproveitar melhor recursos computacionais distribuídos e acelerar o treinamento.
8. Avaliador de exploração: analisar se a exploração do ambiente já foi feita de maneira satisfatória e passar a buscar só explotar a partir de um dado parâmetro de referência ( número de estados totais do ambiente , caso seja discreto). E first 
9. Ajuste automático do epsilon e do decaimento de acordo com o número de episódios e quantidades de estados (se discreto). E proporcional 
10. Ajuste automático da arquitetura da rede, na chamada da função. Onde o usuário escolhe o número quantidade de camadas e do número de neurônios da rede.
11. Avaliação de quantas vezes o estado foi visitado. Usando rede neural. Um epsilon para cada estado. Uma política neural de épsilon.
12. Meta euristica 
13. PER 2: avalia qual foram os episódios com maiores pontuações totais e retorna as experiências vincularas a eles. Foca nos episódios que não deram done. Ou onde a pontuação foi positiva.
14. Aprendizado em paralelo compartilhado. Um vai na frente e o de trás aprende com o erro do da frente e já vai ajustando o da frente com o aprendizado ajustado como um conselheiro que pode tirar um caminho diferente mais eficaz de chegar ao objetivo final.
15. Salvar os parâmetros (pesos) da rede quando a pontuação for 500
16. Quando o agente alcança a pontuação máxima, isso revela que os parâmetros estão muito bons. Portando devem ser salvos, para testar novamente. Em 10 simulações de desempenho. continuar o treinamento pode fazer com que o agente perca os parâmetros ideais e desaprenda o que havia aprendido.
17. Épsilon ajustado por recompensa: se a recompensa for positiva então épsilon diminui, caso a recompensa seja negativa, épsilon aumenta, por exemplo 10%.
18. No caso do cartpole o episódio (finalizar & a pontuação negativa) não é um bom exemplo pra aprender.
19. Épsilon decay duplo 
20. Posso manipular a recompensa em jogos que a recompensa é igual para toda ação.
21. Buffer duplo um com todas as as experiências e outro só com as melhores experiências (500)
22. Aprendizagem em todos os episódios, começa com o agente aprendendo de uma em uma experiência, depois recebe um lote de experiências.
23. Aprendizado proporcional: lote do minibatch, aumenta a cada iteração.
24. Salvar as trajetórias ruins e aprender com elas.
25. Salvar anexo a cada recompensa qual foi a recompensa total da trajetória.
26. Minibatch é parecido com uma revisão de uma parte da matéria. Por isso o aprendizado proporcional pode ser interessante. Representando o minibatch como 10% do batch total.
27. Procurar o centro de computadores da ufc para fazer simulações mais rápidas.
28. Otimizador de parâmetros de treinamento (num_epis): ele para o treinamento quando o valor de erro estiver bem reduzido. Comparando a pontuação máxima de um jogo com a pontuação atual do episódio. Ou avaliando uma função da média dos ultimos k episódios. Apresentar o resultado parcial e perguntar se o cliente quer continuar com o treinamento. Salva os parâmetros da rede quando o algoritmo atinge pontuação máxima.
29. Colocar amostras importantes para o final do buffer
30. Salvar no buffer o episódio completo, ao invés de salvar por experiência e quando for pegar uma amostra, será uma amostra de episódio e não de um número X de experiência
31. Criar um buffer para episódios de 500 pontos e um para todos os episódios, colocar um condicional que escolhe qual buffer vai usar com base em um tamanho mínimo.
32. Buffer que remove amostras idênticas.
