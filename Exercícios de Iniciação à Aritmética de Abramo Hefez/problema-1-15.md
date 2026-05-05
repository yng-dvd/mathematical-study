### Problema 1.15

(a) Quantos múltiplos de 8 existem entre 32 e 8 000, inclusive?
(b) Quantos números pares existem entre 3 211 e 6 321?
(c) Quantas dúzias podemos formar com 180 laranjas? E com 220 laranjas?
(d) Quantas semanas formam 280 dias? E 360 dias?

#### Resposta

* **(a)** Intervalo de multiplicadores: $[4, 1000] \implies (1000 - 4) + 1 = 997$
* **(b)** Espaço aberto $(3211, 6321) \implies$ Intervalo inclusivo de pares: $[3212, 6320] \implies$ Mapeamento de multiplicadores de 2: $[1606, 3160] \implies (3160 - 1606) + 1 = 1555$. 
  * *Raciocínio:* Existem duas formas de resolver. A simples consiste em achar o intervalo inclusivo entre $[3212, 6320]$ e dividir por $2$. A que foi utilizada consiste em mapear a lista de multiplicadores desse intervalo inicial e tomar o intervalo inclusivo a partir dessa lista de fatores. De qualquer forma fez-se o uso da divisão, o que levanta questões estruturais visto que estamos operando sob as propriedades internas do conjunto dos números naturais.
* **(c)** Para 180 laranjas: $[12, 180] \implies [1, 15] \implies (15 - 1) + 1 = 15$ dúzias.
  Para 220 laranjas: $[12, 220] \implies [1, 18] \implies (18 - 1) + 1 = 18$ dúzias.
  * *Raciocínio:* O mesmo do exercício anterior; garantiu-se que o intervalo começasse por um múltiplo de $12$. Ao buscar pelo maior múltiplo de $12$ contido no limite $220$, obteve-se o valor $216$, cujo multiplicador correspondente é $18$. Torna-se complexo conceber uma resolução rigorosa que não exija a operação de divisão ao determinar a cardinalidade de múltiplos em um intervalo fixado.
* **(d)** Para 280 dias: $[7, 280] \implies [1, 40] \implies (40 - 1) + 1 = 40$ semanas.
  Para 360 dias: $[7, 360] \implies [7, 357] \implies [1, 51] \implies (51 - 1) + 1 = 51$ semanas.