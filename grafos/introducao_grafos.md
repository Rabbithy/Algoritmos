<link rel="stylesheet" href="styles.css">

# Introdução aos grafos.
# O que são grafos?
Grafos são estruturas simples usadas para representar algum tipo de relação entre objetos.
Usando essas estruturas, é possível representar mapas, arvores de decisão, caminhos entre pontos etc.
Nas imagens abaixo vemos um grafo onde cada vertice (numerado de forma arbitraria) representa uma esquina, e cada conexão representa uma rua.
<p>
    <img src="assets/mapa_cidade.png" width="330px">
    <img src="assets/grafo_cidade.png" width="370px">
    <p style="font-size: 12px;">Figuras 1 e 2<p>
</p>

# Variações de grafos:
As conexões entre os vertices de um grafo podem sofrer algumas alteções a depender do problema em questão. Duas variações importantes para os grafos são:
- ## Grafos direcionais (Digrafos/Quiver):
    <p>São definidos como grafos onde cada conexão só pode ser percorrida em um único sentido.
    O grafo abaixo representa o fluxo de agua do rio, onde as conexões só podem ser percorridas no sentido indicado por setas.<p>
    <p>
    <img src="assets/rio.png" width="300px">
    <img src="assets/grafo_rio.png" width="250px">
    <p style="font-size: 12px;">Figuras 3 e 4<p>
    </p>
- ## Pesos:
    <p>Em vários grafos são necessários pesos nas conexões, servindo para representar algum atributo da ligação, como distancia entre objetos, tempo de resposta entre computadores em rede, corrente entre dois componentes de um circuito elétrico, etc.</p>
    <p>
    <img src="assets/ilhas.png" width="300px">
    <img src="assets/grafo_ilhas.png" width="280px">
    <p style="font-size: 12px;">Figuras 5 e 6<p>
    </p>

# Representação na memória:
Quando se busca resolver problemas com grafos usando programação, é necessário armazenar as informações do grafo na memoria. A representação de grafos pode ser feita de varios modos. Podemos ver alguns desses modos logo abaixo:
- ## Matriz de adjacencia:
    <p>
    A matriz de adjacencia consiste em uma matriz quadrada de ordem N (sendo N, a quantidade de vertices no grafo), onde um valor localizado na linha X e coluna Y representa a existencia ou não de uma relação entre o vertice X e o vertice Y. Esta é a estrutura base da matriz de adjacencia, mas algumas variações podem ser necessárias de acordo com cada algoritmo/problema.
    </p>
    <p>Na imagem abaixo temos uma matriz de adjacencia representando um grafo direcionado (digrafo):</p>
    <img src="assets/svg/grafo_rio_matriz.svg" width="100%">
- ## Lista de adjacencia:
    <p></p>

# Código


- ## Matriz de adjacencia:

    ``` python
    # Matriz quadrada de ordem N

    matriz = [
        [0, 0, 0, 0],
        [0, 0, 0, 0],
        [0, 0, 0, 0],
        [0, 0, 0, 0]
    ]

    # Definindo relações entre os vertices

    matriz[0][1] = 1    # 0 -> 1
    matriz[0][2] = 1    # 0 -> 2
    matriz[1][3] = 1    # 1 -> 3
    matriz[2][3] = 1    # 2 -> 3

    ```
- ## Lista de adjacencia:
    ``` python
    # Lista de adjacencia composta por outras N listas
    
    lista = [[], [], [], []]

    # Defininfo relações entre os vertices

    lista[0].append(1)
    lista[0].append(2)
    lista[1].append(3)
    lista[2].append(3)
    ```

# Continuação

<div><p>Na proxima página veremos a explicação de alguns algoritmos básicos para começar a criar seus códigos com grafos.</p></div>
<div style="margin-top: 10px;">
    <a class="simple-button" href="menor_caminho.md">Próxima página</a>
</div>