<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [distribution](../../../../../distribution-mathematical-analysis.md) on $(a,b)$ is a continuous [linear functional](../../../../../linear-functional.md) on the [space of test functions](../../../../../space-of-test-functions.md) $\mathcal D(a,b)=C_c^\infty(a,b)$. It has [order of a distribution](../../../../../order-of-a-distribution.md) at most $m$ if, for every [compact set](../../../../../compact-space.md) $K\subset(a,b)$, there is $C_K$ such that

$$
|\langle u,\phi\rangle|\leq C_K\max_{0\leq j\leq m}\|\phi^{(j)}\|_\infty
\qquad(\operatorname{supp}\phi\subseteq K).
$$

The [order of a distribution](../../../../../order-of-a-distribution.md) is the least such $m$. When saying “of order $m$” means merely that this estimate holds, the wording allows a smaller least order.

For each such $K$, the [cutoff function](../../../../../cutoff-function.md) theorem supplies a nonnegative $\chi\in\mathcal D(a,b)$ equal to one near $K$. If $M=\|\phi\|_\infty$ and $\operatorname{supp}\phi\subseteq K$, then $M\chi\pm\phi\geq0$ everywhere. Positivity of the [linear functional](../../../../../linear-functional.md) $V$ therefore gives

$$
0\leq M V(\chi)\pm V(\phi),\qquad
\boxed{|V(\phi)|\leq V(\chi)\|\phi\|_\infty.}
$$

Here $V(\chi)\geq0$ is finite and independent of $\phi$. This is precisely the local bound for an [order-zero distribution](../../../../../order-zero-distribution.md), so the given [positive distribution](../../../../../positive-distribution.md) is continuous on the [space of test functions](../../../../../space-of-test-functions.md). The zero [distribution](../../../../../distribution-mathematical-analysis.md) also satisfies the estimate.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the distribution theory course of the University of Oxford](../../../../split.md)
6. [Distribution theory course of the University of Oxford](../../../../../distribution-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
