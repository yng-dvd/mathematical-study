### Problema 1.5

Usando a propriedade de compatibilidade da adição com a ordem e a transitividade da ordem, mostre que:
Se $a < b$ e $c < d$, então $a + c < b + d$.
Vale a recíproca dessa propriedade?

#### Resposta

Dadas as hipóteses:
1. $a < b$
2. $c < d$

Demonstração:
* Por (1), aplicando a propriedade de compatibilidade da adição com a ordem: $a + c < b + c$
* Por (2), aplicando a propriedade de compatibilidade da adição com a ordem: $b + c = c + b < b + d$
* Unindo as desigualdades por transitividade da ordem: Como $a + c < b + c$ e $b + c < b + d \implies a + c < b + d$.

**Vale a recíproca dessa propriedade? $(a + c < b + d \implies a < b \text{ e } c < d)$?**

Não. Contraexemplo:
Sejam $a = 2, b = 1, c = 3, d = 5$.
$$2 + 3 < 1 + 5 \implies 5 < 6$$
A condição fundamental falha pois $a > b$ ($2 > 1$).