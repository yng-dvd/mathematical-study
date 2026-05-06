# mathematical-study

### AXIOMAS DE PEANO:

Bertrand Russell nos apresenta uma forma refinada dos 5 Axiomas de Peano:

> (1) “0 is a number,” (unidade mínima) <br>
> (2) “The successor of any number is a number,” (noção de sucessor) <br>
> (3) “No two numbers have the same successor,” (garantia da injetividade) <br>
> (4) “0 is not the successor of any number,” (0 não aparece de novo/não é uma progressão cíclica) <br>
> (5) This becomes: Any property which belongs to $x_0$, and belongs to $x_{n+1}$ provided it belongs to $x_n$, belongs to all the $x$’s. (garantia de que o conjunto segue uma ordem conforme as propriedades estipuladas) 
> 
> — Introduction to Mathematical Philosophy by Bertrand Russell. 

Esses axiomas podem ser formalizados da seguinte forma:

1. $N(0)$
2. $\forall n(N(n) \rightarrow N(s(n)))$
3. $\forall n\forall m((N(n) \land N(m) \land (s(n) = s(m))) \rightarrow (n = m))$
4. $\neg\exists n(N(n) \land s(n) = 0)$
5. $(P(0) \land \forall n((N(n) \land P(n)) \rightarrow P(s(n)))) \rightarrow \forall n(N(n) \rightarrow P(n))$

#### Comentário:

O primeiro e o quarto axiomas garantem que haja uma unidade mínima e que junto das propriedades de progressão (2) e (3) não se torne uma progressão cíclica, isto é, que o número mínimo apareça durante a progressão de forma que forçasse uma "reprogressão", já que a progressão se estabelece pela definição de uma unidade mínima e dos sucessores a partir daquela. O quinto axioma garante que os subconjuntos dos Naturais funcione de acordo com os mesmos axiomas que definem os Naturais. Assim, esclarecemos como a ordem se estabelece dentro da progressão do conjunto, de forma que exista uma unidade mínima que não seja sucessor de nenhum número e que tenha um sucessor, este sucessor tendo um sucessor e agora sendo sucessor de uma unidade anterior e assim sucessivamente. Com isso, podemos explorar de forma intuitiva agora as propriedades do conjunto dos Naturais, como as relações de ordem.

#### Propriedade da Adição:

O intervalo garantido $[0, s(0)]$ nos permite traçar que $(s(0))$ está a $1$ uma posição a mais de $0$, pois o intervalo segue uma orientação que parte da esquerda em direção a direita. Com $(s(0))$ a uma posição a direita de $0$, podemos dizer que está a $1$ uma posição a mais de $0$. Para que essa relação seja visualizada usa-se o símbolo de $+$, assim escrevemos que: $s(0) = 0 + 1$, portanto: $s(0) = 1$. Ainda, se buscassemos um sucessor $s(1)$ onde, digamos que,   $s(1) = 1 + 0$, "o sucessor de $1$ está a zero posições de $1$" chegaríamos ao mesmo resultado $1$, pois intuitivamente andar zero posições para a direita significa não sair do lugar. Dessa forma, chegamos a propriedade da comutativa da adição, $0 + 1 = 1 + 0$, ou $a + b = b + a$. De mesma forma, é possível dizer que $(0 + 1) + 1$ e $0 + (1 + 1)$ são iguais, nisto consiste a associativa. Note que se trata de um processo intuitivo, sem o rigor formal para fazer qualquer definição. Por exemplo, o próprio símbolo do número $1$ ou a propriedade da adição não são definidos pelos $5$ axiomas e só serão definidos num processo posterior.

[Em construção...]

### Módulos do Repositório

* **([./Exercícios-de-Iniciação-à-Aritmética-de-Abramo-Hefez](https://github.com/yng-dvd/mathematical-study/tree/5390336a0cebdd207a6f6fb1d99740330d70e396/Exerc%C3%ADcios%20de%20Inicia%C3%A7%C3%A3o%20%C3%A0%20Aritm%C3%A9tica%20de%20Abramo%20Hefez))**
