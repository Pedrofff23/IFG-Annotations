---
{"dg-publish":true,"permalink":"/Faculdade/7 Periodo/Banco de Dados 2/Sub-Notes/NOSQL/","tags":["BD"],"created":"2024-07-11T16:19:09.023-03:00"}
---



## Tópicos
- [[Faculdade/7 Periodo/Banco de Dados 2/Sub-Notes/NOSQL#Por que usar um BD relacional?\|Por que usar um BD relacional?]]
- [[Faculdade/7 Periodo/Banco de Dados 2/Sub-Notes/NOSQL#ACID e Desempenho\|ACID e Desempenho]]
- [[Faculdade/7 Periodo/Banco de Dados 2/Sub-Notes/NOSQL#NOSQL\|NOSQL]]
	- [[Faculdade/7 Periodo/Banco de Dados 2/Sub-Notes/NOSQL#Por que os modelos NOSQL estão em alta?\|Por que os modelos NOSQL estão em alta?]]
	- [[Faculdade/7 Periodo/Banco de Dados 2/Sub-Notes/NOSQL#CAP Consistency, Availability, Partition Tolerance\|CAP Consistency, Availability, Partition Tolerance]]
	- [[Faculdade/7 Periodo/Banco de Dados 2/Sub-Notes/NOSQL#Modelo NOSQL\|Modelo NOSQL]]
		- [[Faculdade/7 Periodo/Banco de Dados 2/Sub-Notes/NOSQL#Tipo documento\|Documuento]]
		- [[Faculdade/7 Periodo/Banco de Dados 2/Sub-Notes/NOSQL#Chave-valor\|Chave-valor]]
		- [[Faculdade/7 Periodo/Banco de Dados 2/Sub-Notes/NOSQL#FAMÍLIA DE COLUNAS\|Família de colunas]]

## Por que usar um BD relacional?

- Por que BD relacionais se tornaram dominantes?
	- Capacidade de armazenar grandes quantidades de dados persistentes, com acesso rápido e fácil
- Controle de concorrência por meio de transações
	- Provê acesso concorrente de múltiplas aplicações ou vários usuários

- Integração compartilhada de BD
	- Aplicações armazenam seus dados em uma única base de dados

- Recuperação após falhas
	- Restaura o BD para um estado anterior ao estado da falha

- Uso de um modelo de dados padrão
	- Dialetos SQL usados por diversos fornecedores são similares

## ACID e Desempenho
Os princípios ACID fortalecem o uso de SGBD relacionais 
- Garantia de **integridade** mesmo sob múltiplos acessos simultâneos;
- Garantia de **preservação do conteúdo** mesmo em caso de falhas graves;
- Garantia de **simplicidade** no projeto e implementação das operações no BD.

# NOSQL

- Gerenciadores que oferecem mecanismos de armazenamento, organização e recuperação que não utilizam a ideia de tabelas ou relações;
- Aparecem a partir da demanda de melhor desempenho
	-Considerando principalmente questões diferentes do uso comum de SGBD Relacionais

## Por que os modelos NOSQL estão em alta?
- Incapacidade de manter o fluxo de acesso ao dados em Bancos relacionais
	- O fluxo de acesso entre modelo relacional e as estruturas de dados na memória de alguma forma não são diretos
- Para acessar os dados no disco, é necessário traduzir a estrutura de dados não atómica da memória para a representação relacional do programa
	- OU seja, a representação da memória e dos softwares não são diretas, exigindo tradução

> [!note] Exemplo
> Uma consulta de uma estrutura que parece ser única na Interface
de um software é dividido em diversas linhas de muitas tabelas relacionais

- BD Relacionais não foram feitos para serem executados em clusters;
- Já os sistemas NoSQL enfatiza a alta disponibilidade, deixando a replicação de forma inerente;
- Algo aplicável também para escalabilidade de ambiente que aumentam ou diminuem o tamanho com facilidade.
- Deixa mais simples o acesso aos Bancos de Dados;
	- Mesmo que o foco seja usar os dados em somente uma máquina
- Deixa mais simples a produtividade por serviços (API), deixando a interação de dados mais livre ou independente para cada serviço;
- Permite lidar eficientemente com o acesso a dados cujo tamanho e desempenho demandam um cluster.

> [!important] Modelos de dados e linguagem de consultas NOSQL
> Modelos e Linguagens possuem *menor prioridade que desempenho e flexibilidade*
> - Não há exigência de um esquema, os dados são então semiestruturados ou autodescritivos. O objetivo é evitar especificar restrições (constraints)
> - No lugar de SQLs, são disponibilizadas para os programadores APIs que fazem CRUD (create, read, update e delete);

## CAP: Consistency, Availability, Partition Tolerance

- **Consistency**
	- *Consistência* entre as *cópias replicadas* do BD
	- Assume um sistema com replicação e que seja distribuído entre os diversos nós

- **Availability**
	- *Disponibilidade* do sistema para *operações de leituras e escrita*
	- *Cada requisição* de *leitura/escrita será processada com êxito*, *ou retornará* com a *indicação* de que *não pode ser realizada*
	
- **Partition Tolerance**
	- Em relação à organização física dos nós de rede que contêm pedaços (shards) do banco de dados
	- O *sistema deve poder continuar a operar* se a *rede tiver uma falha* que *resulte na criação de novas partições*, em que os nós de cada partição possam se comunicar entre si

> [!important] Teorema CAP
> O Teorema CAP afirma que **não é possível garantir as três propriedades** C – A – P **simultaneamente** em um sistema distribuído e com replicação de dados;
> - Se for esse o caso, o projetista ***tem que escolher duas*** das três propriedades para preservar;
> - Em geral sistemas NoSQL optam por enfraquecer o C, gerando uma forma de
consistência chamada consistência eventual;

## Modelo NOSQL
- Modelos de Dados Agregados:
	- Key-value
	- Document Store
	- Famílias de Colunas (wide-columns)   
	- Modelo em Grafos
### Tipo documento
- Em geral, usam XML ou JSON para definir os documentos
- O BD é denominado **coleção**
- Por padrão, *cada documento* na coleção *tem um ObjectID*, fornecido pelo usuário ou gerado pelo sistema;
	- Embora o usuário pode optar por não definir um 
- O modelo orientado a documentos é mais adequado para a representação de objetos complexos.

### MODELAGEM DE DOCUMENTO

- Documentos podem ter:
	- Atributos diferentes entre si
		- Campos que aparecem em um documento mas não aparecem em outro
		- Campos com nomes diferentes
	- Atributos compostos (por exemplo, listas e arrays)
	- Diferentes representações de dados e pertencerem à mesma coleção de documentos
	- Objetos complexos: vários documentos dentro de um outro documento
	- Documentos não possuem atributos vazios
		- Se um dado atributo não for encontrado, supõe-se que ele não é relevante para o documento
	- Documentos permitem que novos atributos sejam criados sem a necessidade de:
		- Definição prévia
		- Alteração nos documentos já existentes
	- ![](https://i.imgur.com/qQu14ls.png)

### Chave-valor
- Cada chave corresponde a um valor, que pode ser um dado simples, um dado estruturado (como uma tupla) ou um desestruturado (como um documento JSON/XML), ou ambos (semiestruturado)
- Tabelas no DynamoDB não têm esquema, mas uma coleção de itens
autodescritivos
- Cada item (valor) consiste de diversos pares (atributo, valor), podendo ser
multivalorados.
- É o tipo de BD NoSQL mais simples de usar a partir da perspectiva de uma API. O
usuário pode:
	- Obter o valor de uma determinada chave;
	- Inserir um valor para uma dada chave;
	- Remover uma chave do BD.
- Valor é um blob ou texto ou JSON ou XML que o BD guarda sem se preocupar ou saber o que há dentro dele
	- É responsabilidade da aplicação entender o que está armazenado
- Já que o acesso é sempre feito pela chave primária:
	- Um bom desempenho pode ser alcançado
	- Podem ser escaláveis facilmente
- Baseia-se em uma hash table contendo uma chave única e um apontador para um item particular de dado
- **Operações**: get(key), put(key, value) e delete( key).
- **Não suporta**:
	-  definição de esquemas;
	-  relacionamentos entre os dados
	-  não possui uma linguagem de consulta.

#### Consultas
- Todos BD chave-valor podem ser consultados pela chave
- Se for preciso consultar algum atributo na coluna de valores, o sistema NoSQL não disponibiliza o recurso
	- Aplicação do usuário se encarregará de fazer esta busca

#### Quando usar chave-valor
- Armazenando informações de sessão
- Perfis de usuário, preferências
- Carrinhos de compra
	- Todas as informações de compras podem ser colocadas no valor onde a chave é userId.

#### Quando não usar chave-valor
- Relacionamentos entre dados
	- Modelar relacionamentos entre diferentes conjuntos de dados ou correlacionar dados entre diferentes conjuntos de chaves
- Transações com múltiplas operações
- Operações de conjuntos
	- Executar operações sobre múltiplas chaves por vez

### Família de colunas