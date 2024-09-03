---
dg-publish: true
dg-show-toc: false

---
## Tópicos

- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Tipos de Grafos#Grafo simples\|Simples]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Tipos de Grafos#Grafo Completo\|Completo]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Tipos de Grafos#Grafo k-regular\|K-regular]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Tipos de Grafos#Grafo Bipartido\|Bipartido]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Tipos de Grafos#Grafo Bipartido Completo\|Bipartido Completo]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Tipos de Grafos#Grafo Cubo-n\|Cubo-n]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Tipos de Grafos#Grafo Ciclo\|Ciclo]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Tipos de Grafos#Grafo Roda\|Roda]] 
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Tipos de Grafos#Multigrafo\|Multigrafo]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Tipos de Grafos#PseudoGrafo\|PseudoGrafo]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Tipos de Grafos#Grafo Imersível\|Imersível]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Tipos de Grafos#Grafo Complementar\|Complementar]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Tipos de Grafos#Grafo Auto-complementar\|Auto-complementar]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Tipos de Grafos#Grafo Conexo\|Grafo Conexo]]


## Grafo simples
- Por meio desta conta podemos calcular a *quantidade de arestas* que um **grafo simples** com **N** nós pode ter:
$$
C(n,2) =  \frac{n\cdot(n-1)}{2}
$$

- E por meio desta conta calculamos o **máximo de grafos simples** com N nós que podem haver:

$$
2^{n \cdot(n-1)/2}
$$

## Grafo Completo

- É um grafo simples em que cada **par de vértices** distintos **possui uma aresta**.

Exemplos de grafos completos 

![](https://i.imgur.com/CKaDw5I.png)

## Grafo k-regular

- **Grafo regular** é um grafo onde cada vértice tem o mesmo número de adjacências.
- O grafo completo kₙ é **(n-1)-regular**
   
Exemplos:

![](https://i.imgur.com/DpDLGpv.png)

![left|300](https://lh7-us.googleusercontent.com/KWmdB752vO91JQF4NsUK7XRldTTJMUZ3zEEnha9FYt_6YO6o4CCg5jYZS2zJucYzGcNHPlnXU__zxKQED2HR2aCyUZnn3smuw10hllXDxZwoPD3CIExlyoGpjaGZnyRgessahIuLKY4v9d6K_hq0nb_-lmkcGscS=s2048)  <br>  <br> <br>  <br> <br> **Este é um grafo 3-regular** 

<br>  <br><br>  <br>

## Grafo Bipartido

- É aquele em que o *conjunto de vértices* pode ser particionado em dois subconjuntos X e Y, tal que cada aresta tem um extremo em X e um em Y.

![](https://i.imgur.com/VQuiFUp.png)

## Grafo Bipartido Completo
- É um grafo bipartido com bipartição (X, Y) em que *cada vértice de X é adjacente a cada vértice de Y.*
- Se |X|=m e |Y|=n, então denotamos tal grafo por Kₘ,ₙ

![center|300](https://upload.wikimedia.org/wikipedia/commons/d/d6/Biclique_K_3_5.svg)

## Grafo Cubo-n
- Um grafo cubo-n de 2ⁿ vértices, denominado Qₙ, é um grafo simples que representa os 2ⁿ strings de n bits. Dois vértices são adjacentes se os strings que eles representam diferem em exatamente uma posição.
![](https://upload.wikimedia.org/wikipedia/commons/f/f8/Hypercubestar.svg)

## Grafo Ciclo
- Um grafo ciclo de n vértices, denominado Cₙ, n ≥ 3, é um grafo simples com n vértices v1, v2, . . . , vn, e arestas v1v2, v2v3, . . ., vn−1vn, vnv1.

![](https://i.imgur.com/WpjG2G7.png)

## Grafo Roda
- Um grafo roda, denominado Wₙ, é um grafo simples com n + 1 vértices que é obtido acrescentado um vértice ao grafo ciclo Cₙ, n ≥ 3, e conectando este novo vértice a cada um dos n vértices de Cₙ.

![](https://i.imgur.com/7nJRdvA.png)

## Multigrafo
- Um multigrafo é um grafo que *não possui laços* mas *pode ter arestas paralelas*. Formalmente, um multigrafo G = (V, E) consiste de um conjunto V de vértices, um conjunto E de arestas, e uma função f de E para {{u, v}|u, v ∈ V, u 6= v}. As arestas e1 e e2 são chamadas múltiplas ou paralelas se f(e1) = f(e2).

![center|400](https://lh7-us.googleusercontent.com/LlpdwSkquCNSE3R0cVSPYw8t_06KYyWz6v6YqAN5uVxBFd_K6_0R9e14kU6qI21Lt5uBhc1-jnuhxQLC89KT3qTBHq6boIkshaBqI1NhXC0FE5fV-1hGDRAfU8rM7fs15ZmOyRYoBzcgBPbUTB1Ay15H5C2z7gcq=s2048)

## PseudoGrafo
- Um pseudografo é um grafo que *pode ter laços e arestas paralelas*. Formalmente, um pseudografo G = (V, E) consiste de um conjunto V de vértices, um conjunto E de arestas, e uma função f de E para {{u, v}|u, v ∈ V }.

**![center|400](https://lh7-us.googleusercontent.com/tZa115TJasduS-E03AW3rZWtnuq24EA2xjY2F3oR08eRolZhR14V6OMK18WTTENqVAD8AUrkTDyKZLxOhJQfYO3eCWrFrNibMCgRIppPHf92yMniLv9vyunykrtX7ZRHGefqaeribs_Ul_jd3VAi_8aRee5qxOUR=s2048)**

## Grafo Imersível

- Um grafo é imersível em uma superfície S se puder ser representado geograficamente em S de tal forma que arestas se cruzem nas extremidades (vértices).

Um *grafo planar* é um grafo que é *imersível no plano*. 

➜ As conexões de uma placa de circuito impresso devem ser representadas por um grafo planar.

## Grafo Complementar
- Seja G um grafo simples.O grafo complementar de G, que denotaremos como F, é definido por V(F) = V(G) e {u,v} e pertencente a E(F) se e somente se {u,v} não pertencer a E(G).

Exemplo:
![]( https://upload.wikimedia.org/wikipedia/commons/2/2f/Petersen_graph_complement.svg)

> [!hint] Dica
> Para encontrar o complemento de um grafo, você preenche todas as arestas que faltavam para obter um grafo completo, e remove todas as arestas que já estavam lá.

## Grafo Auto-complementar
-  Um grafo simples é auto-complementar se é [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Isomorfismo\|isomorfo]] ao seu complemento. 
  
![](https://i.imgur.com/2BHnuHm.png)

## Grafo Conexo
- Um grafo é **conexo** se existe um **caminho** entre *qualquer par de vertices* do grafo.
- Um grafo com apenas um componente é um grafo conectado.

![](https://i.imgur.com/1nZCHXp.png)

### Componentes Conexos
- Os componentes conexos de um grafo são os **subgrafos conexos** maximais deste grafo.
- Exemplo: Este gráfico possui 2 componentes conexos.

![](https://i.imgur.com/H9wCORq.png)

