<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Fredholm alternative for an elliptic Dirichlet problem](../../../../../../fredholm-alternative-for-an-elliptic-dirichlet-problem.md) and part (b) give an inverse $S:Y\to X$ of norm at most $K\geq1$. Choose

$$
\varepsilon=\min\left(1,\frac1{8KC}\right),\qquad
\delta=\min\left(\frac{\varepsilon}{4K},\frac1{4K}\right),\qquad
\varepsilon_0=\frac{\varepsilon}{4K}.
$$

On the closed radius-$\varepsilon$ ball $\mathcal B\subset X$, set $T(v)=S(\mathcal Q(v)+f)$. The stated inequalities give

$$
\|T(v)\|_{C^{2,\alpha}}\leq K(C\varepsilon^2+\delta+\varepsilon_0)
\leq\tfrac58\varepsilon,
$$

and

$$
\|T(v)-T(w)\|_{C^{2,\alpha}}
\leq K(2C\varepsilon+\delta)\|v-w\|_{C^{2,\alpha}}
\leq\tfrac12\|v-w\|_{C^{2,\alpha}}.
$$

Thus $T$ is a [contraction mapping](../../../../../../contraction-mapping.md) of the complete metric space $\mathcal B$ into itself. The [Banach fixed-point theorem](../../../../../../contraction-mapping-theorem.md) gives $u=T(u)$, solving the required [nonlinear elliptic boundary value problem](../../../../../../nonlinear-elliptic-boundary-value-problem.md). This [small-data existence for a nonlinear elliptic Dirichlet problem](../../../../../../small-data-existence-for-a-nonlinear-elliptic-dirichlet-problem.md) also gives uniqueness within this small ball; it does not assert global uniqueness.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
