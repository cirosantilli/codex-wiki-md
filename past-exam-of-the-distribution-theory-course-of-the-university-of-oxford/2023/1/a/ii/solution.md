<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [distributional derivative](../../../../../distributional-derivative.md) of $u$ is defined by

$$
\boxed{\langle u',\phi\rangle=-\langle u,\phi'\rangle\quad(\phi\in\mathcal D(a,b)).}
$$

It is a [distribution](../../../../../distribution-mathematical-analysis.md) because $\phi\mapsto\phi'$ is a continuous map of the [space of test functions](../../../../../space-of-test-functions.md) into itself. If $f\in C^1(a,b)$ represents a [regular distribution](../../../../../regular-distribution.md), [integration by parts](../../../../../integration-by-parts.md) gives

$$
\langle f',\phi\rangle=-\int_a^b f\phi'=\int_a^b f'\phi.
$$

The [boundary term](../../../../../boundary-term.md) vanishes because $\phi$ has [compact support](../../../../../compact-support.md). Thus the [distributional derivative](../../../../../distributional-derivative.md) agrees with the ordinary [derivative](../../../../../derivative.md).

For $\operatorname{supp}\phi\subseteq K$, the assumed [order of a distribution](../../../../../order-of-a-distribution.md) estimate gives

$$
|\langle u',\phi\rangle|\leq C_K\max_{0\leq j\leq m}\|\phi^{(j+1)}\|_\infty
\leq C_K\max_{0\leq j\leq m+1}\|\phi^{(j)}\|_\infty.
$$

Consequently $\boxed{\operatorname{ord}(u')\leq m+1}$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
