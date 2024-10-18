---
{"dg-publish":true,"permalink":"/Faculdade/5 Periodo/Probabilidade/Sub-Notes/Medidas centrais e de dispersão/","tags":["PB"],"created":"2024-10-18T13:31:56.145-03:00"}
---


# Introdução
- **Estatística descritiva**: Nos ajuda a entender melhor um conjunto de dados através de suas características
	- Para *variáveis qualitativas*, as informações podem ser bem resumidas por porcentagens, tabelas de frequência e gráficos.
	- Para as *variáveis quantitativas* (ou numéricas) as três principais características que buscamos num conjunto de dados são:
		- Um valor representativo do conjunto (medida de tendência central); 
		- Uma medida de dispersão ou variação; 
		- A natureza ou forma da distribuição dos dados.
# Medidas de Tendência Central
**São medidas que determinam valores típicos ou representativos de um conjunto de dados. **

## Média Aritmética

$$
	\overset{-}x = \frac{1}{2} \sum_{i=1}^\limits{n} = \frac{x1 + x2 + x3 + ...}{n}
$$


## Média Ponderada
$$
\overset{-}x = \frac{x1*n1 + x2*n2 + x3*n3 + ... + nk*nk}{n1 + n2 + n3 + ... + nk} = \frac{1}{n} \sum_{i=1}^\limits{k} n_{i} * k_{j}
$$


## Mediana
- Para Casos Impares

$$
	MD = x(\frac{n+1}{2}) 
$$

- Para Casos Pares

$$
	MD = \frac{x{\frac{n}{2}} + x(\frac{n}{2}+1)}{2} 
$$

## Moda

- Pegar o valor que possui a maior frequência.
- Existem amostras que possuem mais que uma moda, sendo classificadas como *multimodais*

## Média para dados agrupados

- Como podemos proceder para obter a média, mediana e moda desse conjunto de dados sendo que **não conhecemos todos os valores** obtidos na amostra?
- Nesse caso, nada mais natural do que eleger o *ponto médio do intervalo* para este papel.

$$
\overset{-}x = \frac{1}{2} \sum_{i=1}^\limits{n}n_{i}x_{i}^*
\qquad ou \qquad \overset{-}x = \sum_{i=1}^\limits{n}f_{i}x_{i}^*
$$
- Dessa forma, em cada classe i, tomaremos o ponto médio do intervalo (x ∗ i ) e calculamos a média ponderada

## Mediana para dados agrupados
$$
Md = l_{i} + \frac{1}{n_{i}} \left(\frac{n}{2}-N_{a}\right)*h_{i}
$$
- a classe **i** é a classe da mediana (obtida verificando o número de elementos da amostra); 
- **Li** é o limite inferior da classe i; 
- **Ni** é o número de elementos (frequência) da classe i;
- **n** é o número de elementos da amostra; 
- **Na** é a frequência acumulada da classe anterior à classe i; 
- **hi** é a amplitude da classe i.

## Moda para dados agrupados

$$
Mo = l_{i} + \frac{h_{i}*f_{p}}{f_{a}+f_{p}'}
$$

- a classe **i** é a classe modal, isto é, a classe com maior frequência;
- **i** é o limite inferior da classe i; 
- **hi** é a amplitude da classe i; 
- **fa** é a frequência relativa da classe anterior a classe i; 
- **fp** é a frequência relativa da classe posterior a classe i.


