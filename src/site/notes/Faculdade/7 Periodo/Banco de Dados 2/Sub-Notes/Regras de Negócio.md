---
{"dg-publish":true,"permalink":"/Faculdade/7 Periodo/Banco de Dados 2/Sub-Notes/Regras de Negócio/","tags":["BD"],"created":"2024-06-26T00:24:10.600-03:00"}
---

## Tipos de Restrições
- **Regras de Integridade:**
	- Estoque com valores negativos
- **Regras de Automatização:**
	- Caso um estoque chegue em um valor mínimo, exigindo uma mensagem solicitando reposição
## Regras de Negócio no SGBD
### Vantagens em mantê-las no SGBD
- Simplificação no código da aplicação;
- Simplificação nas manutenção das regras;
- Maior garantia de integridade das informações.
### Desvantagens
- Dificuldade de migração entre SGBDs. Softwares que pregam a heterogeneidade entre SGBDs podem não conseguir tal feito;
- Em alguns casos pode sobrecarregar o SGBD.
## Violação de Restrições
### Inserção:
- Restrição de **Domínio**: valor fora do domínio
- Restrição de **Chave**: valor já existe
- Restrição de **integridade** de entidade: se chave for null
- Restrição de **integridade referencial**: se chave estrangeira referencia tupla inexistente
***Ação padrão: rejeitar inserção (com explicação)***

### Remoção
- Tupla excluída é referenciada por chaves estrangeiras
- ***Soluções:***
	- Ação padrão: bloqueia/rejeitar a remoção (com explicação)
	- Propagar remoção de tuplas que violem uma restrição de integridade referencial – Efeito cascata
	- Modificar o valor da chave estrangeira para nulo