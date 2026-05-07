### Problema 1.16

> Seja $c \neq 0$.
> 
> (a) Mostre que: $0 < c < 2 \cdot c < 3 \cdot c < 4 \cdot c < 5 \cdot c$.  
> (b) Mostre que vale a recíproca da propriedade acima, isto é, que se $a \cdot c < b \cdot c$, então $a < b$.

#### Resposta

**(a) Resolução:** Se $c \neq 0$, $c \in \mathbb{N}$ e zero não é sucessor de nenhum número, então $c$ só pode ser maior do que zero, valendo $0 < c$. Pela propriedade da compatibilidade da multiplicação com a ordem, então $0 \cdot n < c \cdot n = 0 < c \cdot n$, como sabemos que $0 < c$, e para todo $n \neq 1$: $c \cdot n = c + \dots + c$, $n$ vezes, então $c < c \cdot n$, logo: $0 < c < c \cdot n$, para todo $c \neq 0$ e todo $n \neq 1$ elementos de $\mathbb{N}$.

**(b) Resolução:** $a \cdot c < b \cdot c$, sendo $c = 0$, então $a \cdot c = b \cdot c$. Como $a \cdot c < b \cdot c$, temos uma contradição, logo: $c \neq 0$.

Como $a \cdot c$ soma o número $c$ "$a$" vezes e $b \cdot c$ soma o número $c$ "$b$" vezes para que $c + \dots + c < c + \dots + c$: se $c + \dots + c = c + \dots + c$ então $a = b$ então $a \cdot c = b \cdot c$ o que contradiz a premissa, de mesmo modo, se $c + \dots + c > c + \dots + c$ então $a > b$ então $a \cdot c > b \cdot c$, o que contradiz a premissa. Logo, se $a \cdot c < b \cdot c$ então $a < b$.