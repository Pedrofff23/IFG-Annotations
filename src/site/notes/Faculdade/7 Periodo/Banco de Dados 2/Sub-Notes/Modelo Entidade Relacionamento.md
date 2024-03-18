---
{"dg-publish":true,"tags":["BD"],"permalink":"/Faculdade/7 Periodo/Banco de Dados 2/Sub-Notes/Modelo Entidade Relacionamento/","dgPassFrontmatter":true}
---

## Atributo e Entidade
### Atributo
**São propriedades que descrevem uma entidade**
#### Exemplo:
```mermaid
flowchart LR
E1 --> Nome:João
E1 --> Idade:28
E1 --> Sexo:Masculino
E1 --> Fone:556223208787
```
#### Composto Vs Simples
- **Atributo Composto** representam atributos básico com significado independente
```mermaid
flowchart LR
E1 --> Nome:João
E1--> Idade:28
E1--> Sexo:Masculino
E1-->Endereço 
Endereço -->Lote:34
Endereço -->CEP:74200160
```
#### Valores possíveis
- **Valor NULL**
	- Desconhecido ou não aplicável
- **Chave primaria**
	- Atributo que possui *valor único* para cada entidade (instância)
		- Ex. Nome da companhia, identidade do empregado
- **Chave composta:**
	- Pode ser formada por vários atributos
		- Registro do Veículo: Número de Registro e Estado
### Entidade
**Define um conjunto de entidades que têm os mesmos atributos (propriedades)**
- Exemplo: O que uma entidade projeto possui?
	- Nome
	- Número
	- Localização
	- Departamento
- *Entidade Fraca*: Não tem chave própria
- *Padrões de nome* 
	- Tipo entidade: Nomes em singular e tudo maiúsculo
	- Atributo: Primeira letra maiúscula
	- Papeis: Tudo minúsculo
### Relacionamentos
 **Associações entre duas ou mais entidades distintas**

#### Tipos de Relacionamento
##### Auto-Relacionamento
![](https://i.imgur.com/vWV8S7N.png)
##### Ternário
![](https://i.imgur.com/aS66Lss.png)
##### Atributo em relacionamento
![](https://i.imgur.com/NMQYiCs.png)

#### Imagens de diagramas
![](https://i.imgur.com/FyXVjLr.png)
![](https://i.imgur.com/ENtfaFn.png)
