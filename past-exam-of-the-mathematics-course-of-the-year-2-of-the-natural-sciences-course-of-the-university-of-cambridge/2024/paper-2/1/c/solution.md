<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For sufficiently smooth functions satisfying the same [boundary conditions](../../../../../boundary-condition.md), [integration by parts](../../../../../integration-by-parts.md) gives the boundary form

$$
\begin{aligned}
\langle f,\mathcal Lg\rangle-\langle\mathcal Lf,g\rangle
&=\int_{-L}^L\left[-f^*(pg')'+(pf^{*\prime})'g\right]dx\\
&=\left[p\bigl(f^{*\prime}g-f^*g'\bigr)\right]_{-L}^{L}.
\end{aligned}
$$

The stated endpoint relation annihilates this expression. This proves the required [self-adjoint differential operator](../../../../../self-adjoint-differential-operator.md) identity; for the usual regular [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md), separated real [boundary conditions](../../../../../boundary-condition.md) give a self-adjoint realization on its domain.

In this problem the transformed [diffusive flux](../../../../../diffusive-flux.md) is $J=-e^{-\lambda t}py'$. Thus the physical [boundary conditions](../../../../../boundary-condition.md) are

$$
\boxed{py'(\pm L)=0,}
$$

equivalently $y'(\pm L)=0$ when the endpoint values of $p$ are positive. In particular $pf'=pg'=0$ at the endpoints, which makes the boundary form vanish directly. The [inner product](../../../../../inner-product-split.md) used here is the ordinary integral; the weight $w$ enters the [generalized eigenvalue problem](../../../../../generalized-eigenvalue-problem.md), not this boundary-form calculation.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
