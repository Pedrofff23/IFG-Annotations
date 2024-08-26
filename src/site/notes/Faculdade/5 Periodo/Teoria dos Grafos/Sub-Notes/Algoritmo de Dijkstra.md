---
{"dg-publish":true,"permalink":"/Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Algoritmo de Dijkstra/","created":"2024-07-08T21:12:33.344-03:00"}
---


## Todos os passos

```mermaid
flowchart LR
	a:::visited -->|2| b
	a -->|1| c
	b -->|1| d
	c-->|3| d
	c-->|4|e
	d--->|2|f
	e-->|2|f

	classDef visited fill:#f96,color:#000000
```
|   iter  |  visitado   | a     | b     | c     | d     | e     | f   |
| --- | --- | ----- | ----- | ----- | ----- | ----- | --- |
| 1º  | a   | (0,-) | **(2,a)** | **(1,a)** | ∞     | ∞     | ∞   |



```mermaid
flowchart LR
	a:::visited -->|2| b
	a -->|1| c
	b -->|1| d
	c:::visited -->|3| d
	c-->|4|e
	d--->|2|f
	e-->|2|f

	classDef visited fill:#f96,color:#000000
```
|   iter  | visitado    | a     | b     | c     | d     | e     | f   |
| --- | --- | ----- | ----- | ----- | ----- | ----- | --- |
| 1º  | a   | (0,-) | (2,a) | (1,a) | ∞     | ∞     | ∞   |
| 2º  | c   | (0,-) | (2,a) | (1,a) | **(4,c)** | **(5,c)** | ∞   |



```mermaid
flowchart LR
	a:::visited -->|2| b
	a -->|1| c
	b:::visited -->|1| d
	c:::visited -->|3| d
	c-->|4|e
	d--->|2|f
	e-->|2|f

	classDef visited fill:#f96,color:#000000
```
| iter | visitado | a     | b     | c     | d     | e     | f   |
| ---- | -------- | ----- | ----- | ----- | ----- | ----- | --- |
| 1º   | a        | (0,-) | (2,a) | (1,a) | ∞     | ∞     | ∞   |
| 2º   | c        | (0,-) | (2,a) | (1,a) | (4,c) | (5,c) | ∞   |
| 3º   | b        | (0,-) | (2,a) | (1,a) | *(3,b)* | (5,c) | ∞   |


```mermaid
flowchart LR
	a:::visited -->|2| b
	a -->|1| c
	b:::visited -->|1| d
	c:::visited -->|3| d
	c-->|4|e
	d:::visited--->|2|f
	e-->|2|f

	classDef visited fill:#f96,color:#000000
```
| iter | visitado | a     | b     | c     | d       | e     | f   |
| ---- | -------- | ----- | ----- | ----- | ------- | ----- | --- |
| 1º   | a        | (0,-) | (2,a) | (1,a) | ∞       | ∞     | ∞   |
| 2º   | c        | (0,-) | (2,a) | (1,a) | (4,c)   | (5,c) | ∞   |
| 3º   | b        | (0,-) | (2,a) | (1,a) | (3,b)   | (5,c) | ∞   |
| 4º   | d        | (0,-) | (2,a) | (1,a) | (3,b) | (5,c) | **(5,d)**  |


```mermaid
flowchart LR
	a:::visited -->|2| b
	a -->|1| c
	b:::visited -->|1| d
	c:::visited -->|3| d
	c-->|4|e
	d:::visited--->|2|f
	e:::visited-->|2|f

	classDef visited fill:#f96,color:#000000
```
| iter | visitado | a     | b     | c     | d       | e     | f   |
| ---- | -------- | ----- | ----- | ----- | ------- | ----- | --- |
| 1º   | a        | (0,-) | (2,a) | (1,a) | ∞       | ∞     | ∞   |
| 2º   | c        | (0,-) | (2,a) | (1,a) | (4,c)   | (5,c) | ∞   |
| 3º   | b        | (0,-) | (2,a) | (1,a) | (3,b)   | (5,c) | ∞   |
| 4º   | d        | (0,-) | (2,a) | (1,a) | (3,b) | (5,c) | (5,d)  |
| 5º   |   e      | (0,-) | (2,a) | (1,a) | (3,b) | (5,c) | (5,d)  |
| 6º   |     f     | (0,-) | (2,a) | (1,a) | (3,b) | (5,c) | (5,d)  |


```mermaid
flowchart LR
	a:::visited -->|2| b
	a -->|1| c
	b:::visited -->|1| d
	c:::visited -->|3| d
	c-->|4|e
	d:::visited--->|2|f
	e:::visited-->|2|f
	f:::visited
	classDef visited fill:#f96,color:#000000
```
| iter | visitado | a     | b     | c     | d       | e     | f   |
| ---- | -------- | ----- | ----- | ----- | ------- | ----- | --- |
| 1º   | a        | (0,-) | (2,a) | (1,a) | ∞       | ∞     | ∞   |
| 2º   | c        | (0,-) | (2,a) | (1,a) | (4,c)   | (5,c) | ∞   |
| 3º   | b        | (0,-) | (2,a) | (1,a) | (3,b)   | (5,c) | ∞   |
| 4º   | d        | (0,-) | (2,a) | (1,a) | (3,b) | (5,c) | (5,d)  |
| 5º   |   e      | (0,-) | (2,a) | (1,a) | (3,b) | (5,c) | (5,d)  |
| 6º   |     f     | (0,-) | (2,a) | (1,a) | (3,b) | (5,c) | (5,d)  |

### Resposta menor custo
Rota de A até F = A->B->D->F

