<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First suppose that $X$ is separable. Choose a norm-dense sequence $(x_n)$ in $B_X$. On every norm-bounded subset of $X$, a countable norm-dense subset $(f_n)$ of $B_{X^*}$ in the weak-star topology separates points, and

$$
d(x,y)=\sum_{n=1}^\infty2^{-n}
\frac{|f_n(x-y)|}{1+|f_n(x-y)|}
$$

metrizes the [weak topology](../../../../../../weak-topology-split.md). Indeed, convergence for all $f_n$, boundedness, and weak-star density imply convergence for every $f\in X^*$. Thus a [weakly compact set](../../../../../../weakly-compact-set.md) $K$ is a compact metric space and hence is sequentially compact.

For general $X$, take a sequence $(x_n)$ in $K$ and let

$$
Y=\overline{\operatorname{span}}\{x_n:n\geq1\}.
$$

The space $Y$ is separable and norm closed. The [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) shows both that $Y$ is weakly closed in $X$ and that its own weak topology is the subspace topology inherited from $X$. Hence $K\cap Y$ is weakly compact and, by the separable case, contains a weakly convergent subsequence of $(x_n)$. Its limit lies in $K\cap Y$. Therefore every weakly compact subset of a Banach space is [weakly sequentially compact](../../../../../../weakly-sequentially-compact-set.md), which is one direction of the [Eberlein-Šmulian theorem](../../../../../../eberlein-smulian-theorem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
