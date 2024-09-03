---
dg-publish: true
tags:
  - BD
---

## Consultas Básicas em SQL

**Formado Básico**
	- Select (lista de atributos)
	- From (lista de tabelas)
	- Where (condição)

Exemplos:
```sql
SELECT datanascimento, endereço
	FROM EMPREGADO
	WHERE pnome= ‘John’ AND minicia = ‘B’ and unome=‘Smith’
```

$$
π_{datanascimento,endereco}\hspace{2mm} \text{σ (pnome= ‘John’ AND minicia = ‘B’ and unome=‘Smith’)}^{(EMPREGADO)}
$$

```sql
SELECT E.FNAME, E.LNAME, S.FNAME, S.LNAME
FROM EMPREGADO AS E, EMPREGADO AS S
WHERE E.COD_GERENTE = S.CPF
```
---
Nas tabelas e nos resultados as tuplas duplicadas podem aparecer, uu seja, *não há eliminação automática das linhas duplicadas*.
Para isso utilizamos:
- **Distinct**
	- Select distinct nome from empregado
- **União**
- **Exceção**
- **Interseção**

#### Joins
O parênteses na clausula **from** forma uma *única tabela*: como resultado da clausula join
```sql
SELECT FNAME, LNAME, ENDERECO
FROM (EMPREGADO JOIN DEPARTAMENTE ON DNO=DNUMBER)
WHERE DNAME=‘PESQUISA’
```
#### Like, between e order by
- Operador LIKE
```sql
select * from aluno where nome like 'Jorge‘
select * from aluno where nome like '%a%‘
```
- Operador BETWEEN
```sql
select * from pagamento where valor between 20 and 32
```
- Operador ORDER BY
```sql
select * from aluno order by nome asc/desc
```

#### Consultas Aninhadas
```sql
select * from aluno where id in (select id_aluno from pagamento);
select * from aluno where id not in (select id_aluno from
pagamento)
```

#### Junção entre tabelas
```sql
select a.nome as NomeAluno, a.id as Matrícula, p.data, p.valor
from aluno as a inner join pagamento as p on a.id=p.id_aluno

select a.nome as NomeAluno, a.id as Matrícula, p.data, p.valor
from aluno as a left join pagamento as p on a.id=p.id_aluno

select a.nome as NomeAluno, a.id as Matrícula, p.data, p.valor
from aluno as a right join pagamento as p on a.id=p.id_aluno
```

#### Funções Agregadas e Agrupamento


```sql
Função SUM
select sum(valor) from pagamento

Função MAX
Select max(valor) from pagamento

Função AVG
select avg(valor) from pagamento

Função MIN
Select min(valor) from pagamento

Função COUNT
select count(*) from pagamento
select count(distinct data) from pagamento
```

#### Cláusula GROUP BY
Exemplo tabela de alunos:

| Matricula | Nome | Sexo | Cr  |
| --------- | ---- | ---- | --- |
| 1         | A    | F    | CC  |
| 2         | B    | M    | CC  |
| 3         | C    | M    | CC  |
| 4         | D    | F    | MC  |
| 5         | E    | M    | MC  | 

```sql
SELECT CR, COUNT(*), AS NUM_ALUNOS FROM ALUNOS
GROUP BY CR
```
Depois da pesquisa:

| CR  | NroAlunos |
| --- | --------- |
| CC  | 3         |
| MC  | 2         | 

##### Restrições em Group By
```sql
SELECT CR, COUNT(*) AS NUM_ALUNOS FROM ALUNOS
GROUP BY CR
HAVING NUM_ALUNOS > 3
```


> [!important] Having e Where
> A cláusua **where** restringe a **relação**
O agrupamento (*GROUP BY e HAVING*), *agrupa o resultado da relação*.

---
### Querys feitas na sala

```sql
SELECT pnumber,dnum,lname addres, bdate
	FROM projeto as p, departamento as d, empregado as e
	WHERE plocation='Anapolis' and d.num = p.dnum and d.gerente=e.cpf
```

```sql
SELECT p.pnumber, d.dnum, e.lname, e.address, e.bdate
	FROM projeto p
	INNER JOIN departamento d ON d.dnum = p.dnum
	INNER JOIN empregado e ON d.gerente = e.cpf
	WHERE p.plocation = 'Anapolis';
```

```sql
SELECT *
	FROM D INNER JOIN P on D.num = P.dnum
	INNER JOIN  E on 
```