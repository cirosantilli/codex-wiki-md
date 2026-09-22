<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A symmetric function $k:\mathcal X\times\mathcal X\to\mathbb R$ is a [positive-semidefinite kernel](../../../../../../positive-semidefinite-kernel.md) when, for every $m$, every $x_1,\ldots,x_m\in\mathcal X$, and every $c\in\mathbb R^m$,

$$
\sum_{i,j=1}^mc_ic_jk(x_i,x_j)\geq0.
$$

Equivalently, every associated [kernel matrix](../../../../../../kernel-matrix.md) is a [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md).

A [Reproducing kernel Hilbert space](../../../../../../reproducing-kernel-hilbert-space.md) $\mathcal H$ on $\mathcal X$ is a [Hilbert space](../../../../../../hilbert-space-split.md) of real-valued functions such that every point-evaluation map $f\mapsto f(x)$ is continuous. The [Riesz representation theorem](../../../../../../riesz-representation-theorem.md) then gives a function $k(x,\cdot)\in\mathcal H$ satisfying the [reproducing property](../../../../../../reproducing-property.md)

$$
f(x)=\langle f,k(x,\cdot)\rangle_{\mathcal H}.
$$

Its reproducing kernel is $k(x,y)=\langle k(x,\cdot),k(y,\cdot)\rangle_{\mathcal H}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
