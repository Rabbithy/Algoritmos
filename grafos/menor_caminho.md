# Introdução:
A busca de menor caminho é uma questao classica da teoria dos grafos, sendo assim, existem varios algoritmos já criados para resolver esse tipo de problema. Abaixo temos a explicação de alguns deles:

- # Dijkstra:
    O algoritmo de Dijkstra consiste em, a partir de um vertice X de um grafo, encontrar o menor caminho até um vertice Y. - Para isso ele separa os vertices do grafo em dois tipos: os percorridos e os não percorridos.
    - Então depois de definir estes dois grupos ele percorre todos os vertices adjacentes (vizinhos) do vertice atual.
    Para cada vertice vizinho ele amazena o peso em uma lista separada (caso o grafo não possua pesos explicitos então é considerado como peso igual à 1). 
    - Apos percorrer os vertices adjacentes, os mesmos são adicionados no grupo de vertices percorridos, ou seja, não é mais necessário calcular a distancia dele.
    - A segunda parte do algoritmo consiste em repetir o processo para cada um dos vertices adjacentes iniciais, até encontrar o vertice Y.

    - "O algoritmo considera um conjunto S de menores caminhos, iniciado com um vértice inicial I. A cada passo do algoritmo busca-se nas adjacências dos vértices pertencentes a S aquele vértice com menor distância relativa a I e adiciona-o a S e, então, repetindo os passos até que todos os vértices alcançáveis por I estejam em S. Arestas que ligam vértices já pertencentes a S são desconsideradas."
    <img src="assets/animacao_ilhas.gif" width="300px">
- ## Dijkstra recursivo:
                                                                                                    
- ## Dijkstra não recursivo:

- # A*:

