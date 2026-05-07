# mathematical-study

Este repositório dedica-se à formalização e estudo de conceitos fundamentais da aritmética e lógica matemática.

---
# Conjunto dos Números Naturais
## 1. Identidade e suas Propriedades

Definimos a identidade de um número e como ela se comporta através do símbolo ($=$).

* **Reflexividade:** Dado um número $x$ qualquer, $x$ é igual a ele mesmo.
    $$\forall x(x = x)$$
* **Simetria:** Para qualquer que seja o número $x$ e o número $y$, se $x = y$, então $y = x$.
    $$\forall x \forall y [(x = y) \rightarrow (y = x)]$$
* **Transitividade:** Para quaisquer números $x, y, z$, se $(x = y)$ e $(y = z)$, então $(x = z)$.
    $$\forall x \forall y \forall z [(x = y) \land (y = z) \rightarrow (x = z)]$$

---

## 2. Axiomas de Peano

Baseado na forma refinada apresentada por **Bertrand Russell** em *Introduction to Mathematical Philosophy*:

> (1) “0 is a number,” (unidade mínima)  
> (2) “The successor of any number is a number,” (noção de sucessor)  
> (3) “No two numbers have the same successor,” (garantia da injetividade)  
> (4) “0 is not the successor of any number,” (0 não aparece de novo/não é uma progressão cíclica)  
> (5) This becomes: Any property which belongs to $x_0$, and belongs to $x_{n+1}$ provided it belongs to $x_n$, belongs to all the $x$’s. (garantia de que o conjunto segue uma ordem conforme as propriedades estipuladas)

### Formalização Lógica

1. $N(0)$
2. $\forall n(N(n) \rightarrow N(s(n)))$
3. $\forall n\forall m((N(n) \land N(m) \land (s(n) = s(m))) \rightarrow (n = m))$
4. $\neg\exists n(N(n) \land s(n) = 0)$
5. $(P(0) \land \forall n((N(n) \land P(n)) \rightarrow P(s(n)))) \rightarrow \forall n(N(n) \rightarrow P(n))$

#### Comentário
O primeiro e o quarto axiomas garantem que haja uma unidade mínima e que junto das propriedades de progressão (2) e (3) não se torne uma progressão cíclica, isto é, que o número mínimo apareça durante a progressão de forma que forçasse uma "reprogressão", já que a progressão se estabelece pela definição de uma unidade mínima e dos sucessores a partir daquela. O quinto axioma garante que os subconjuntos dos Naturais funcione de acordo com os mesmos axiomas que definem os Naturais. Assim, esclarecemos como a ordem se estabelece dentro da progressão do conjunto, de forma que exista uma unidade mínima que não seja sucessor de nenhum número e que tenha um sucessor, este sucessor tendo um sucessor e agora sendo sucessor de uma unidade anterior e assim sucessivamente. Com isso, podemos explorar de forma intuitiva agora as propriedades do conjunto dos Naturais, como as relações de ordem.

---

## 3. Propriedades

### 3.1 Adição

O intervalo garantido $[0, s(0)]$ nos permite traçar que $(s(0))$ está a $1$ uma posição a mais de $0$, pois o intervalo segue uma orientação que parte da esquerda em direção a direita. Com $(s(0))$ a uma posição a direita de $0$, podemos dizer que está a $1$ uma posição a mais de $0$. 

Para que essa relação seja visualizada usa-se o símbolo de $+$, assim escrevemos que: $s(0) = 0 + 1$, portanto: $s(0) = 1$. Ainda, se buscassemos um sucessor $s(1)$ onde, digamos que, $s(1) = 1 + 0$, "o sucessor de $1$ está a zero posições de $1$" chegaríamos ao mesmo resultado $1$, pois intuitivamente andar zero posições para a direita significa não sair do lugar. 

Dessa forma, chegamos a propriedade da comutativa da adição, $0 + 1 = 1 + 0$, ou $a + b = b + a$. De mesma forma, é possível dizer que $(0 + 1) + 1$ e $0 + (1 + 1)$ são iguais, nisto consiste a associativa. 

> **Nota:** Trata-se de um processo intuitivo, sem o rigor formal para fazer qualquer definição. Por exemplo, o próprio símbolo do número $1$ ou a propriedade da adição não são definidos pelos $5$ axiomas e só serão definidos num processo posterior.

### 3.2 Subtração

A subtração é definida como a inversa da adição. Ainda que não fornecida, essa definição nos ajuda a traçar certas relações entre a adição e a subtração:
* (a + b) - b = a
* (b - a) + a = b, para b >= a;
* (a - b) - c = a - (b + c), para a >= b;
* a - (b - c) = (a - b) + c
* (a - b) - c != a - (b - c) Ex.: (3 - 1) - 2 = 0 e 3 - (1 - 2) = ∅ 

> **Nota:** A operação da subtração não tem as propriedades da comutativa e associativa.

### 3.3 Múltiplos

É considerado múltiplo de a ∈ N e k ∈ N todo produto b tal que b = a*k. Assim:

* a é o fator;
* k é o multiplicador;
* b é o múltiplo (o produto).

Assim, podemos dizer que, se b = 0, então k = 0 ou a = 0.
> **Nota:** Como b = 0 * k é sempre igual 0 para qualquer que seja k ∈ N, dizemos que b (o múltiplo) de zero é apenas o próprio zero. Assim, o zero é múltiplo de qualquer número (k), mas só o zero é múltiplo de zero.
---

## 4. Teoremas

### Teorema 1: Se $x \neq y$, então $s(x) \neq s(y)$.

**Prova:** Concedendo que se x != y, então s(x) = s(y) fosse verdade, então x != y poderia ser falso ou verdadeiro, se x != y for falso, então x = y é verdadeiro, logo, s(x) = s(y) não pode ser falso, com base no Axioma 3. Se (x != y) for verdadeiro, então significa que (x = y) é falso, por consequência, como o consequente é falso no Axioma 3, o antecedente deve ser falso para que continue verdadeiro e aplicável ao número, assim, a conjunção deve ser falsa. Como se trata do conjunto dos Naturais sabemos que N(0) é verdadeiro, logo, s(x) = s(y) deve ser falso. Portanto, s(x) != s(y).

### Teorema 2: $s(n) \neq n$

**Prova Formal:**
$N(0) \land \forall n(N(n) \rightarrow N(s(n))) \land \forall n\forall m((N(n) \land N(m) \land (s(n) = s(m))) \rightarrow (n = m)) \land \neg\exists n(N(n) \land s(n) = 0) \land (P(0) \land \forall n(N(n) \land P(n) \rightarrow P(s(n))) \rightarrow \forall n(N(n) \rightarrow P(n)) \vdash \forall n(s(n) \neq n)$

1.  $N(0)$ (premissa)
2.  $\forall n(N(n) \rightarrow N(s(n)))$ (premissa)
3.  $\forall n\forall m((N(n) \land N(m) \land (s(n) = s(m))) \rightarrow (n = m))$ (premissa)
4.  $\neg\exists n(N(n) \land s(n) = 0)$ (premissa)
5.  $(P(0) \land \forall n(N(n) \land P(n) \rightarrow P(s(n)))) \rightarrow \forall n(N(n) \rightarrow P(n))$ (premissa)
6.  $\quad N(n) \land s(n) \neq n$ (hipótese para indução)
7.  $\quad \quad s(s(n)) = s(n)$ (hipótese para reductio)
8.  $\quad \quad N(s(n)) \rightarrow N(s(s(n)))$ ($\forall E$ 2)
9.  $\quad \quad N(s(n))$ ($\rightarrow E$ 6, 2)
10. $\quad \quad N(s(s(n)))$ ($\rightarrow E$ 9, 8)
11. $\quad \quad (N(s(n)) \land N(s(s(n))) \land (s(s(n)) = s(n))) \rightarrow s(n) = n$ ($\forall E$ 3)
12. $\quad \quad s(n) = n$ ($\rightarrow E$ 9, 10, 7, 11 + simetria)
13. $\quad \quad \bot$ (6, 12)
14. $\quad s(s(n)) \neq s(n)$ ($\neg I$ 7-13)
15. $\forall n(N(n) \land s(n) \neq n \rightarrow s(s(n)) \neq s(n))$ ($\forall I$ 6-14)
16. $\quad s(0) = 0$ (hipótese para reductio)
17. $\quad N(0)$ (R1)
18. $\quad N(0) \land s(0) = 0$ ($\land I$ 16, 17)
19. $\quad \exists n(N(n) \land s(n) = 0)$ ($\exists I$ 18)
20. $\quad \neg\exists n(N(n) \land s(n) = 0)$ (R4)
21. $\quad \bot$ (19, 20)
22. $s(0) \neq 0$ ($\neg I$ 16-21)
23. $s(0) \neq 0 \land \forall n(N(n) \land s(n) \neq n \rightarrow s(s(n)) \neq s(n))$ ($\land I$ 22, 15)
24. $\forall n(N(n) \rightarrow s(n) \neq n)$ ($\rightarrow E$ 5, 23)

### Teorema 3: Se $x \neq 0$, então $x = s(u)$
*[Em construção...]*

---
## Módulos do repositório

[./Exercícios de Iniciação à Aritmética - Abramo Hefez](https://github.com/yng-dvd/mathematical-study/tree/716095894534dfdf6815a9679f26c1b5a6f81ea4/Exerc%C3%ADcios%20de%20Inicia%C3%A7%C3%A3o%20%C3%A0%20Aritm%C3%A9tica%20de%20Abramo%20Hefez)
