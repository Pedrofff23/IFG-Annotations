---
{"dg-publish":true,"permalink":"/Faculdade/7 Periodo/Banco de Dados 2/Sub-Notes/Normalização/","tags":["BD"],"created":"2024-10-18T13:31:56.148-03:00"}
---


> [!summary] Definição
> É definido como uma *série de passos* em um projeto de um banco de dados que permite um *armazenamento consistente e um acesso eficiente* em bancos de dados relacionais.

Contudo, existem **medidas informais de qualidade** do projeto de um
esquema relacional:
- Atributos das *relações semanticamente compatíveis*
- *Ausência de valores redundantes* nas relações (inexistência de
anomalias de atualização)
- *Número reduzido* de *valores nulos* nas relações
- *Sem* possibilidade de *gerar tuplas espúrias/falsas*

## Definição Funcional
Os valores de Y dependem funcionalmente ou são determinados por X, ou seja:
- O atributo X é uma chave Primária que determina Y;
- Os valores do componente Y de uma tupla em R dependem dos
(ou são determinados pelos) valores do componente X;

#### Regras de Inferência para DF
O responsável pelas regras de negócio junto com o DBA, definem algumas DFs, mas
outras podem ser inferidas;
**Regras**:
1. Regra Aumentativa: X → Y então XZ → YZ
2. Regra Transitiva: X → Y, Y → Z então X → Z
3. Regra de Decomposição: X → YZ então X → Y
4. Regra de União: X→Y, X→Z então X→YZ e nunca X→A e Y→B irá gerar XY→AB
5. Regra da dependência parcial: XY→A então X→A

## Formas Normais
A princípio são feitos vários testes para garantir que a relação se encontra em uma certa forma normal;
**Objetivos**:
- Minimizar redundância
- Minimizar anomalias de alteração de dados

### Primeira Forma Normal
Tem que ser atômico, ou seja, não poder multivalorados ou compostos.

### Segunda Forma Normal
Acontece somente com chave composta

Um atributo deve depender das duas chaves primarias(dependencia funcional), se ele depender apenas de uma se cria uma nova tabela

### Terceira Forma Normal
Chave primaria simples, todos atributos devem depender da chave primaria, senão gera uma nova tabela

### Quarta Forma Normal
Uma relação viola a 4FN quando é identificado uma Dependência Multivalorada

Muita redundancia