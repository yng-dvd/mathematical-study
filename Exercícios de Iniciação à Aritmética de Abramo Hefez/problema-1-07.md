### Problema 1.7

Mostre que se $c \le a < b$, então $a - c < b - c$.

#### Resposta

Hipóteses:
1. $c \le a$
2. $a < b$

Se $c = 0$, então:
$$a < b \implies a - c < b - c \implies a - 0 < b - 0 \implies a < b$$

Se $c = n < a$:
$$a < b \implies a - n < b - n$$

Por indução, aplicando o passo sucessor:
$$a < b \implies a - n < b - n \implies (a - n) - 1 < (b - n) - 1 \implies a - (n + 1) < b - (n + 1)$$