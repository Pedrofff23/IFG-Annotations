---
dg-publish: true
---
## Tópicos
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Árvores#Teoremas\|Teoremas]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Árvores#Corolário\|Corolário]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Árvores#Aresta de Corte\|Aresta de Corte]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Árvores#Árvore geradora\|Árvore geradora ]]
	- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Árvores#Algoritmo de Krustal\|Algoritmo de Krustal]]
	- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Árvores#Algoritmo de Prim\|Algoritmo de Prim]]
> [!info]  Definições
> 1. Um grafo é **acíclico** se não contém circuito.
> 2. **Árvore** é um grafo **acíclico** e **conexo**.

## Teoremas
1. Quaisquer dois vértices de uma árvore estão ligados por um único caminho.
   
2. Se G é uma árvore então |E(G)| = |V (G)|−1.

## Corolário
1. Seja G uma árvore, x e y dois vértices de G tais que e = (x, y) ∉ E(G). Então G + e contém um único circuito.
2.  Toda árvore com pelo menos dois vértices tem pelo menos dois vértices de grau um.

## Aresta de Corte
- Uma aresta de corte *e* é de corte se, e somente se, não existe caminho em *G - e* ligando os extremos de *e*.
 -  Em outras palavras uma aresta e = w é de corte se:
	 - *e* **é o único caminho ligando** *u* a *v*
	 - **não existe circuito contendo *e***

> [!summary] Teorema
> Um **grafo conexo é uma árvore** se, e somente se, **toda aresta é de corte**

## Árvore geradora 
- Uma árvore geradora de um grafo G é um subgrafo gerado de G que é uma árvore.
- **OBS:**
	- *Todo grafo conexo contém uma árvore geradora*

### Árvore geradora  de custo mínimo
Se G é um grafo com peso nas aresta então:
- w(e) indica o peso da arestas e.
- w(G) indica o peso total do grafo G.

#### Teoremas
1. A floresta de k árvores na qual tem um total de n vértices tem n - k arestas.
	- k = 4 e n = 18
	- m = n - k = 18 - 4 = 14 arestas
1. **(Formula de Cayley)**: Seja n ∈ IN. Considere Kn o [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Tipos de Grafos#Grafo Completo\|grafo completo]] com n vértices. Então o número de árvores geradoras de Kn é dado por **τ(G) = n^n−2**.
2. Seja G um grafo conexo então o número de árvores geradoras é τ (G) =τ(G−e) +τ (G \ e)
3. **Kirchhoff?**


#### Algoritmo de Krustal
> [!info] Observações  
> - Os custos são números inteiros arbitrários (positivos e negativos).
> - O problema tem solução se e somente se o grafo é [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Tipos de Grafos#Grafo Conexo\|conexo]].

Ideia básica:
- Seleciona a **aresta de menos peso** que conecta duas árvores de uma floresta.
- Repita o processo até que todos os vértices estejam conectados sempre preservando a invariante de se ter uma árvore.

[[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Algoritmo de Krustal\| Exemplo do Algoritmo de Krustal]]

#### Algoritmo de Prim

Ideia básica:
- Tomando como vértice inicial A, crie uma **fila de prioridades** classificada pelos pesos das arestas conectando A.
- Repita o processo até que todos os vértices tenham sido visitados.

[[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Algoritmo de Prim\|Exemplo do Algoritmo de Prim ]]