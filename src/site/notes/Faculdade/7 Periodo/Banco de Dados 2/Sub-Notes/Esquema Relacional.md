---
{"dg-publish":true,"permalink":"/Faculdade/7 Periodo/Banco de Dados 2/Sub-Notes/Esquema Relacional/","tags":["BD"],"created":"2024-06-26T00:24:10.600-03:00"}
---

*O modelo relacional representa um banco de dados como um conjunto de
relações*
## Conceitos do Modelo Relacional
- Linhas de uma relação (tabela) = tuplas
- Cabeçalho de cada coluna = atributo
- Conjunto de valores que pode aparecer em cada coluna = domínio
## Restrições de Integridade Básicas
- **Restrição de domínio:** Especificam que o valor de cada atributo A de uma relação deve ser um valor do domínio, dom(A)
- **Restrição de chave:** 
	- Um esquema de relação pode ter mais de uma chave → chaves candidatas
	- Uma delas é indicada como chave primária e as chaves alternativas
- **Restrição de valores NULL:**
	- Se é permitido valores null ou não
## Restrições de Integridade do Esquema
### Entidade
Nenhum componente de uma chave primária pode ser nulo;
### Referencial
Usada para manter a consistência entre tuplas de duas relações;
### Esquema de um BD Relacional
![](https://i.imgur.com/s7Lfpof.png)
