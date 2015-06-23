Trabalho 2 - SCC0112 - ICMC-USP
==============

O conteúdo abaixo foi obtido diretamente do [Moodle USP](http://disciplinas.stoa.usp.br/pluginfile.php/318330/mod_resource/content/2/2o%20Trabalho%20pratico.pdf).

Desenvolvido por:

- Pedro Góes
- Marcelo Montanher

Especificação
==============
O objetivo desse trabalho é analisar o desempenho de um sistema de hierarquia de memórias através de
simulações.
Para tanto, o grupo deve escolher um programa que faça essa simulação de cache e que seja possível
configurar:
 Memória Principal
 Memória Cache
o Com a possibilidade de variar o tamanho da cache
o Com a possibilidade de variar o tamanho do bloco
o Com a possibilidade de variar a função de mapeamento
o Com possibilidade de variar as políticas de substituição
o Com a possibilidade de definir vários níveis
 Programa ou traces com referências a memória
O grupo deve definir quatro (4) arquivos de programa ou de trace (o que o simulador suportar) que
possuam acessos à memória com as seguintes características:
1. Não possua princípios de localidade espacial e temporal
2. Possua princípios de localidade temporal
3. Possua princípios de localidade espacial
4. Possua princípios de localidade temporal e espacial
Com base nos arquivos com as características acima, o grupo deve definir uma arquitetura base,
considerando os seguintes fatores:
 Tamanho da cache
 Tamanho do bloco
 Função de mapeamento
 Algoritmo de substituição
 Número e tipo de caches
A partir dessa arquitetura base, deve-se variar os fatores, um de cada vez, com pelo menos 3 níveis.
Exemplo de arquitetura base:
 Tamanho da cache : 128 palavras
 Tamanho do bloco: 1 palavra
 Função de mapeamento: direto
 Algoritmo de substituição: FIFO
 Número e tipo de caches: 1 cache unificada
Variando o primeiro fator, pode-se definir outras 2 arquiteturas:
 Tamanho da cache : 256 palavras
 Tamanho do bloco: 1 palavra
 Função de mapeamento: direto
 Algoritmo de substituição: FIFO
 Número e tipo de caches: 1 cache unificada
 Tamanho da cache : 512 palavras
 Tamanho do bloco: 1 palavra
 Função de mapeamento: direto
 Algoritmo de substituição: FIFO
 Número e tipo de caches: 1 cache unificada
Variando-se o segundo fator, pode-se definir outras 2 arquiteturas:
 Tamanho da cache : 128 palavras
 Tamanho do bloco: 2 palavras
 Função de mapeamento: direto
 Algoritmo de substituição: FIFO
 Número e tipo de caches: 1 cache unificada
 Tamanho da cache : 128 palavras
 Tamanho do bloco: 4 palavras
 Função de mapeamento: direto
 Algoritmo de substituição: FIFO
 Número e tipo de caches: 1 cache unificada
Deve-se repetir esse procedimento para todos os fatores, resultando em um total de 11 arquiteturas (1
arquitetura base + 10 arquiteturas que variam os fatores)
Com a definição das arquiteturas e dos programas/traces que serão executados, deve-se executar as
simulações onde cada arquitetura deve executar os 4 programas/traces, obtendo como resposta da
simulação a taxa de acertos na cache (se for cache multinível deve-se considerar a taxa de acerto em cada
nível).
Com os resultados em mãos, o grupo deve fazer uma análise dos seguintes pontos:
1. Relação da taxa de acerto (hit rate) com o tamanho da cache. Com isso, conclua sobre o impacto do
tamanho da cache na taxa de acerto
2. Relação da taxa de acerto (hit rate) com o tamanho do bloco. Com isso, conclua sobre o impacto do
tamanho do bloco na taxa de acerto
3. Relação da taxa de acerto (hit rate) com o nível de associatividade. Com isso, conclua sobre o
impacto da associatividade da cache na taxa de acerto
4. Relação da taxa de acerto (hit rate) com o algoritmo de substituição. Com isso, conclua sobre o
impacto do algoritmo de substituição na taxa de acerto
5. Relação da taxa de acerto (hit rate) com o número de caches. Com isso, conclua sobre o impacto da
quantidade de caches na taxa de acerto
A memória principal deve ser grande o suficiente para conter o programa/trace que será simulado.
De maneira a apresentar os resultados, o grupo deve entregar uma monografia contendo:
 Uma breve introdução sobre o simulador escolhido (quem fez, como funciona, etc.)
 Os arquivos de programa ou de trace utilizados
 As configurações das arquiteturas
 Gráficos e a análise dos gráficos
 Conclusão
A entrega do mesmo trabalho (mesmo simulador, mesmos arquivos de programas/trace, mesmas
arquiteturas) por dois ou mais grupos resultará na nota zero para os grupos envolvidos.
Qualquer dúvida em relação a execução desse trabalho deve-se entrar em contato com a professora ou
com os estagiários PAE.