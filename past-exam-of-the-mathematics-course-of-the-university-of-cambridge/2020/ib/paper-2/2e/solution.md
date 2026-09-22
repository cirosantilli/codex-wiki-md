<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

Write $D(f)=\mathbb C\setminus f^{-1}(0)$. The zero and constant-one polynomials give $D(0)=\varnothing$ and $D(1)=\mathbb C$. Also,

$$
D(f)\cap D(g)=D(fg),
$$

so $\tau$ is closed under finite intersections. Every nonzero one-variable complex polynomial has only finitely many roots, and every finite subset $\{a_1,\ldots,a_m\}$ is the zero set of $\prod_j(z-a_j)$. Consequently $\tau$ is exactly the [cofinite topology](../../../../../cofinite-topology.md): its open sets are the empty set and the complements of finite sets. An arbitrary union of such sets is again empty or has finite complement, so $\tau$ is a [topology](../../../../../topology-split.md).

The [product topology](../../../../../product-topology.md) on $X\times Y$ is the topology with basis

$$
\{U\times V:U\subseteq X\text{ open},\ V\subseteq Y\text{ open}\}.
$$

The proposed complement need not be open. Take

$$
g(z,w)=z-w.
$$

Then $g^{-1}(0)$ is the diagonal. If its complement were open, a point such as $(0,1)$ would have a basic neighbourhood $U\times V$ contained in that complement. But $U$ and $V$ are nonempty cofinite subsets of $\mathbb C$, so $U\cap V\ne\varnothing$. For $t\in U\cap V$, the point $(t,t)$ belongs both to $U\times V$ and to the diagonal, a contradiction. Hence

$$
\boxed{\mathbb C^2\setminus g^{-1}(0)\text{ is not always product-open}}.
$$

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
