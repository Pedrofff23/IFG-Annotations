---
{"dg-publish":true,"permalink":"/Faculdade/5 Periodo/Sistema Operacionais/Sub-Notes/Processos/","created":"2024-12-26T10:28:39.594-03:00"}
---


> [!important] 
> - E/S duram uma eternidade para a CPU
> - Nesse tempo, a CPU pode processar outras coisas
> - Como controlar toda essa concorrência/simultaneidade? **Processos e threads**.

## Processos
- **Todo** software em execução no SO é um **processo**;
- Uma CPU executa um **único processo** por vez. Mas como a alternância *é muito rápida*, dá-se a ilusão de processos serem executados paralelamente – **pseudoparalelismo**.
- Um **algoritmo escalonador/agendador** (scheduling algorithm) é o componente que realiza a alternância
- Um programa é uma série de passos para realizar uma tarefa
	- Está em memória secundária, inerte
- Um processo é uma instância de um programa em execução.
	- Contém o contexto da CPU, das variáveis, recursos de E/S (estado do processo) e o programa em si
	- Ele está em memória primária
- 