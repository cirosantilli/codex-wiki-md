<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume first that $X_n\xrightarrow dX$. Because all variables take values in the compact interval $[-C,C]$, each monomial $x^k$ agrees there with a bounded continuous function on $\mathbb R$. The [bounded moment criterion for weak convergence](../../../../../../bounded-moment-criterion-for-weak-convergence.md) in this case begins with

$$
\mathbb E[X_n^k]\longrightarrow\mathbb E[X^k]
$$

for every natural number $k$.

Conversely, suppose all moments converge. Let $f$ be bounded and continuous. By the [Weierstrass approximation theorem](../../../../../../weierstrass-approximation-theorem.md), for every $\varepsilon>0$ there is a polynomial $P$ with

$$
\sup_{|x|\leq C}|f(x)-P(x)|\leq\varepsilon.
$$

Moment convergence implies $\mathbb E[P(X_n)]\to\mathbb E[P(X)]$, while

$$
|\mathbb E[f(X_n)-P(X_n)]|leq\varepsilon,
\qquad
|\mathbb E[f(X)-P(X)]|\leq\varepsilon.
$$

Taking the limit superior and then $\varepsilon\downarrow0$ proves $\mathbb E[f(X_n)]\to\mathbb E[f(X)]$, which is [convergence in distribution](../../../../../../convergence-in-distribution.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
