<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We prove the [polynomial nonvanishing below the field size](../../../../../../polynomial-nonvanishing-below-the-field-size.md) by [mathematical induction](../../../../../../mathematical-induction.md) on $n$. The case $n=1$ is the [Lagrange root bound over a field](../../../../../../lagrange-root-bound-over-a-field.md): a nonzero polynomial of degree below $p$ cannot have all $p$ elements of $\mathbb F_p$ as roots.

For the induction step, suppose that $P$ vanishes on all of $\mathbb F_p^n$ and write

$$
P(x_1,\ldots,x_n)=\sum_{j=0}^{p-1}P_j(x_1,\ldots,x_{n-1})x_n^j.
$$

The upper limit is valid because the [total degree of a polynomial](../../../../../../total-degree-of-a-polynomial.md) is less than $p$. Fixing the first $n-1$ variables produces a univariate polynomial of degree below $p$ which vanishes at every $x_n\in\mathbb F_p$. It is therefore the zero polynomial, so every $P_j$ vanishes on all of $\mathbb F_p^{n-1}$. Each $P_j$ also has total degree below $p$, and the induction hypothesis gives $P_j=0$ for every $j$. Thus $P=0$.

Taking the [contrapositive](../../../../../../contrapositive.md), every nonzero such $P$ has some $a\in\mathbb F_p^n$ for which

$$
\boxed{P(a)\ne0.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 147](../../../paper-147-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
