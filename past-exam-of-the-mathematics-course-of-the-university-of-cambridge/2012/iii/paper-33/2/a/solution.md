<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $Y_i$ be [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) with [moment-generating function](../../../../../../moment-generating-function.md) finite on an open interval about $0$. Put

$$
\Lambda(\theta)=\log\mathbb E e^{\theta Y_1},\qquad I(x)=\sup_{\theta\in\mathbb R}\{\theta x-\Lambda(\theta)\},
$$

allowing $\Lambda=+\infty$ outside its finite domain. The [Cramér theorem](../../../../../../cramer-s-theorem.md) states that $\bar Y_n=n^{-1}\sum_{i=1}^nY_i$ satisfies a [large deviation principle](../../../../../../large-deviation-principle.md) with speed $n$ and good [rate function](../../../../../../rate-function.md) $I$, the [Legendre transform of a cumulant-generating function](../../../../../../legendre-transform-of-a-cumulant-generating-function.md). Explicitly, for every closed set $F$ and open set $O$,

$$
\limsup_{n\to\infty}\frac1n\log\mathbb P(\bar Y_n\in F)\leq-\inf_{x\in F}I(x),\qquad
\liminf_{n\to\infty}\frac1n\log\mathbb P(\bar Y_n\in O)\geq-\inf_{x\in O}I(x).
$$

Here $\log0=-\infty$ and $\inf\varnothing=+\infty$. The [rate function](../../../../../../rate-function.md) is lower semicontinuous and its finite sublevel sets are compact. **The exponential-moment hypothesis is essential for this form of the [Cramér theorem](../../../../../../cramer-s-theorem.md).**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
