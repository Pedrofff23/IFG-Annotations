---
{"dg-publish":true,"permalink":"/Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Caminhos e Ciclos/","created":"2024-10-18T13:31:56.148-03:00"}
---


## Tópicos
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Caminhos e Ciclos#Caminhos\|Caminhos]]
	- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Caminhos e Ciclos#Passeio\|Passeio]]
	- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Caminhos e Ciclos#Caminho\|Caminho]]
- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Caminhos e Ciclos#Ciclos\|Ciclos]]
	- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Caminhos e Ciclos#Trilha/Trajeto\|Trilha/Trajeto]]
	- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Caminhos e Ciclos#Circuito/Trajeto fechado\|Circuito/Trajeto fechado]]
	- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Caminhos e Ciclos#Ciclo\|Ciclo]]
	- [[Faculdade/5 Periodo/Teoria dos Grafos/Sub-Notes/Caminhos e Ciclos#Exemplos\|Exemplos]]

## Caminhos
### Passeio
- Um passeio em um grafo G = (V, E) consiste de uma *sequência finita* alternada de *vértices e arestas*.
- Um passeio com **k** vértices possui **k-1 arestas**.
### Caminho
- Um **caminho** em um grafo G = (V, E) *é um passeio* em que todos os seus **vértices** são **distintos**.

![](https://www.ime.usp.br/~pf/algoritmos_para_grafos/aulas/figs/Sedgewick-Wayne/TinyNetwork-x.png)

0-2-7-3-6 é um caminho simples

## Ciclos 
### Trilha/Trajeto
- É um **passeio** em que **todas** as suas **arestas são distintas**.

### Circuito/Trajeto fechado
- É um **trajeto** em que o *vértice inicial* e o *vértice final* são **iguais**.

### Ciclo
- É um **circuito** em que *todos os vértices* são **distintos** (exceto o primeiro e o último).

**OBS: grafo acíclico é aquele que não possui ciclos**

### Exemplos
#### Exemplo 1:

![center|300](https://i.imgur.com/GVOIAAM.png)

**A sequência {c,a,d,e,c}:**
1. É uma trilha
2. É um circuito
3. É um ciclo

#### Exemplo 2:

![](https://i.imgur.com/iFCBiAG.png)

- Possíveis caminhos:
	1. E → B → D→E
	2. A → C → D → E → B → A
	3. B → D → E → B → C
	4.  A → B → C → D → B → A


| Passeio | Caminho | Circuito |
| ------- | ------- | -------- |
| 1. Sim  | Sim     | Sim      |
| 2. Sim  | Sim     | Sim      |
| 3. Sim  | Não     | Não      |
| 4. Sim  | Não     | Não         |
