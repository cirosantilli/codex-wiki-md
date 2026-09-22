<h1 id="3d/solution">Solution</h1>

↑ **Parent:** [3D](../3d.md)

A [sequence](../../../../../sequence.md) $(x_n)$ is a [convergent sequence](../../../../../convergent-sequence.md) with limit $x$ if

$$
\forall\varepsilon>0\ \exists N\in\mathbb N\
\forall n\ge N:\quad |x_n-x|<\varepsilon.
$$

The index $N$ may depend on $\varepsilon$, but must work for every later term.

Fix $\varepsilon>0$. Choose $N$ such that $|x_i-x|<\varepsilon/2$ for $i\ge N$, and put

$$
C=\sum_{i=1}^{N-1}|x_i-x|.
$$

This is a fixed finite number. For $n\ge N$, the [triangle inequality](../../../../../triangle-inequality.md) gives

$$
\left|\frac1n\sum_{i=1}^nx_i-x\right|
\le\frac1n\sum_{i=1}^n|x_i-x|
\le\frac Cn+\frac{n-N+1}{n}\frac{\varepsilon}{2}
\le\frac Cn+\frac{\varepsilon}{2}.
$$

Choose $n$ sufficiently large that $C/n<\varepsilon/2$ as well. The error is then less than $\varepsilon$, proving

$$
\boxed{\frac1n\sum_{i=1}^nx_i\longrightarrow x.}
$$

**Taking successive arithmetic averages preserves the limit.** This is the [Cesaro theorem for convergent sequences](../../../../../cesaro-theorem-for-convergent-sequences.md): any troublesome initial terms contribute only a fixed numerator divided by $n$.

## ↑ Ancestors (10)

1. [3D](../3d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
