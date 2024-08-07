---
{"dg-publish":true,"permalink":"/Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Árvores/","created":"2024-08-06T08:23:31.502-03:00"}
---

## Tópicos
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Árvores#Teoremas\|Teoremas]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Árvores#Corolário\|Corolário]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Árvores#Aresta de Corte\|Aresta de Corte]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Árvores#Árvore geradora\|Árvore geradora ]]
	- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Árvores#Algoritmo de Krustal\|Algoritmo de Krustal]]
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

#### Algoritmo de Krustal
> [!info] Observações  
> - Os custos são números inteiros arbitrários (positivos e negativos).
> - O problema tem solução se e somente se o grafo é [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Tipos de Grafos#Grafo Conexo\|conexo]].

Idéia básica:
- Seleciona a aresta de menos pedo que conecta duas árvores de uma floresta.
- Repita o processo até que todos os vértices estejam conectados sempre preservando a invariante  de se ter uma árvore.

[[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Exemplo Algoritmo de Krustal\|Exemplo Algoritmo de Krustal]]: