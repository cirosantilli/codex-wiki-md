<h1 id="12g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [metric space](../../../../../../metric-space.md) $(X,d)$, [uniform continuity](../../../../../../uniform-continuity.md) means

$$
\forall\varepsilon>0\ \exists\delta>0\ \forall x,y\in X:
\quad d(x,y)<\delta\ \Longrightarrow\ |f(x)-f(y)|<\varepsilon.
$$

The choice of $\delta$ is independent of the points. A [Lipschitz continuous](../../../../../../lipschitz-continuity.md) function satisfies $|f(x)-f(y)|\leq Ld(x,y)$ for one finite constant $L\geq0$. Choosing $\delta=\varepsilon/(L+1)$ proves **Lipschitz continuity implies uniform continuity**.

Let $(x_n)$ be a [Cauchy sequence](../../../../../../cauchy-sequence.md). For a given $\varepsilon>0$, uniform continuity supplies $\delta>0$, and the Cauchy property supplies $N$ with $d(x_m,x_n)<\delta$ for $m,n\geq N$. Then $|f(x_m)-f(x_n)|<\varepsilon$, so $(f(x_n))$ is Cauchy in $\mathbb R$. By [completeness of the real numbers](../../../../../../completeness-of-the-real-numbers.md), **$(f(x_n))$ converges**, even if the original sequence has no limit in $X$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12G](../../12g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
