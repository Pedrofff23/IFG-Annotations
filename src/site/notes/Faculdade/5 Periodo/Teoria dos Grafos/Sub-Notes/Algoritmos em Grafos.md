---
{"dg-publish":true,"permalink":"/Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Algoritmos em Grafos/","created":"2024-12-26T10:28:40.204-03:00"}
---


## Tópicos
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Algoritmos em Grafos#Matriz de Incidência\|Matriz de Incidência]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Algoritmos em Grafos#Matriz de Adjacência\|Matriz de Adjacência]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Algoritmos em Grafos#Algoritmos de busca em Grafos\|Algoritmos de busca em Grafos]]
	- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Algoritmos em Grafos#Algoritmo de Dijkstra\|Algoritmo de Dijkstra]]
	- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Algoritmos em Grafos#Algoritmo de Floyd\|Algoritmo de Floyd]]

## Matriz de Incidência

- Representação com V (vértices) e E (arestas)
- Como montar:

![](https://i.imgur.com/unxNtlI.png)

|     | e1  | e2  | e3  | e4  | e5  | e6  | e7  |
| --- | --- | --- | --- | --- | --- | --- | --- |
| v1  | 1   | 1   | 0   | 0   | 1   | 0   | 1   |
| v2  | 1   | 1   | 1   | 0   | 0   | 0   | 0   |
| v3  | 0   | 0   | 1   | 1   | 0   | 0   | 1   |
| v4  | 0   | 0   | 0   | 1   | 1   | 2   | 0   | 

## Matriz de Adjacência

- Representação com apenas V (vértices) 

![](https://i.imgur.com/unxNtlI.png)

|     | v1  | v2  | v3  | v4  |
| --- | --- | --- | --- | --- |
| v1  | 0   | 2   | 1   | 1   |
| v2  | 2   | 0   | 1   | 0   |
| v3  | 1   | 1   | 0   | 1   |
| v4  | 1   | 0   | 1   | 1   |

# Algoritmos de busca em Grafos
Vamos descrever dois algoritmos de busca em grafos:
- **Busca em largura**
	- *Põe* na fila um vértice qualquer u de G e marque-o como alcançado
	- ```portugol
		Enquanto fila ≠ ∅ faça
		* v ← elemento da frente da fila (retire v da fila)
		* para toda aresta (v,w), tal que w ainda não foi alcançado, marque w como alcançado e põe w na fila.

- **Busca em profundidade**
	- *Empilhe* um vértice qualquer u de G e marque-o como alcançado
	- ```portugol
		Enquanto pilha ≠ ∅ faça
		* v ← elemento do topo-da-pilha
		* se existe aresta (v,w), tal que w ainda não foi alcançado, então marque w como alcançado e empilhe w; senão desempilha v.

## Problema do caminho mínimo
### Algoritmo de Dijkstra

- Escolhido um **vértice** como **raiz da busca**, este algoritmo *calcula o custo mínimo deste vértice para todos os demais vértices* do grafo.

- O algoritmo pode ser usado sobre grafos orientados, ou não, e admite que todas as arestas possuem **pesos não negativos**.

[[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Algoritmo de Dijkstra\|Exemplo de Resolução]]

### Algoritmo de Floyd
- Seja D = (V,A) um grafo dirigido, *possivelmente com custos negativos* nas arestas, mas **sem circuitos negativos**. O algoritmo de Floyd-Warshall (1959, 1962) determina a *distância* entre *cada par de vértices de D*.
- É um algoritmo que resolve o problema de *calcular o caminho mais curto entre todos os pares de vértices* em um grafo dirigido e valorado (com peso).

[[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Algoritmo de Floyd\|Exemplo de Resolução]]