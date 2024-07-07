---
{"dg-publish":true,"permalink":"/Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Algoritmos em Grafos/","created":"2024-06-26T00:24:10.600-03:00"}
---


## Tópicos
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Algoritmos em Grafos#Matriz de Incidência\|Matriz de Incidência]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Algoritmos em Grafos#Matriz de Adjacência\|Matriz de Adjacência]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Algoritmos em Grafos#Algoritmos de busca em Grafos\|Algoritmos de busca em Grafos]]

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
```portugol
Enquanto fila ≠ ∅ faça
	* v ← elemento da frente da fila (retire v da fila)
	* para toda aresta (v,w), tal que w ainda não foi alcançado, marque w como alcançado e põe w na fila.
```
- **Busca em profundidade**
	- *Empilhe* um vértice qualquer u de G e marque-o como alcançado
	- ```portugol
		Enquanto pilha ≠ ∅ faça
		* v ← elemento do topo-da-pilha
		* se existe aresta (v,w), tal que w ainda não foi alcançado, então marque w como alcançado e empilhe w; senão desempilha v.

