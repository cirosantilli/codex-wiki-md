<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

On upper exit, $b\leq S_T\leq b+c$; on lower exit, $-a-c\leq S_T\leq-a$. With $p=\mathbb P(S_T\geq b)$ and $\mathbb ES_T=0$,

$$
pb-(1-p)(a+c)\leq0
\leq p(b+c)-(1-p)a.
$$

Solving gives

$$
\frac a{a+b+c}\leq p\leq\frac{a+c}{a+b+c}.
$$

Moreover $(S_T+a)(S_T-b)\geq0$, so $\mathbb ES_T^2\geq ab$, which is stronger than the requested lower bound. Also $S_T\in[-a-c,b+c]$, and hence

$$
(S_T+a+c)(b+c-S_T)\geq0.
$$

Taking expectations and using $\mathbb ES_T=0$ gives $\mathbb ES_T^2\leq(a+c)(b+c)$, stronger than the requested upper bound. Since

$$
ab\geq\frac{ab(a+b)}{a+b+c},
\qquad
(a+c)(b+c)\leq
\frac{(a+c)(b+c)(a+b+2c)}{a+b+c},
$$

the two stated estimates follow from part a.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
