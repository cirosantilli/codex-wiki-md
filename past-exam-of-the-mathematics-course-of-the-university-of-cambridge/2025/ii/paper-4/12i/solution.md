<h1 id="12i/solution">Solution</h1>

↑ **Parent:** [12I](../12i.md)

A subset $A$ of a metric space $X$ is a [nowhere dense set](../../../../../nowhere-dense-set.md) when

$$
\operatorname{int}\overline A=\varnothing.
$$

Equivalently, every nonempty open set contains a nonempty open subset disjoint from $A$.

The [Baire category theorem](../../../../../baire-category-theorem.md) says that if $X$ is a complete metric space and $G_1,G_2,\ldots$ are open dense subsets of $X$, then $\bigcap_{n\geq1}G_n$ is dense in $X$. Equivalently, no nonempty open subset of $X$ is a countable union of nowhere-dense sets.

To prove it, take a nonempty open set $V$. Since $G_1$ is open and dense, there is a closed ball

$$
\overline B(x_1,r_1)\subset V\cap G_1
$$

with $0<r_1<2^{-1}$. Inductively, openness and density of $G_{n+1}$ allow us to choose

$$
\overline B(x_{n+1},r_{n+1})
\subset B(x_n,r_n)\cap G_{n+1},
\qquad 0<r_{n+1}<2^{-(n+1)}.
$$

The balls are nested, and for $m>n$ their centres satisfy

$$
d(x_m,x_n)<r_n<2^{-n}.
$$

Thus $(x_n)$ is Cauchy and has a limit $x\in X$. Every closed ball contains the tail of the sequence, so it contains $x$. Hence

$$
x\in V\cap\bigcap_{n\geq1}G_n.
$$

As $V$ was arbitrary, the intersection is dense.

## ↑ Ancestors (10)

1. [12I](../12i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
