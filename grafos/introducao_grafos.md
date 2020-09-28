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
Quando se busca resolver problemas com grafos usando programação, é necessário armazenar as informações do grafo na memoria. Existem varios modos e tecnicas para fazer isso. Abaixo temos alguns desses modos:

- ## Lista de adjacencia:
    ``` python
    """
    0 -> 1
    0 -> 2
    1 -> 3
    2 -> 3
    """
    lista = [[1, 2], [3], [3], []]
    ```

- ## Matriz de adjacencia:
    <img src="assets/svg/grafo_rio_matriz.svg">
    
    ``` python
    """
    0 -> 1
    0 -> 2
    1 -> 3
    2 -> 3
    """
    matriz = [
        [0, 1, 1, 0],
        [0, 0, 0, 1],
        [0, 0, 0, 1],
        [0, 0, 0, 0]
    ]
    ```