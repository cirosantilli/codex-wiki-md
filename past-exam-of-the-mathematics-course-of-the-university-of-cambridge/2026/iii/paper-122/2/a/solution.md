<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
N=\left\lfloor c\left(\frac{k}{\log k}\right)^{4/3}\right\rfloor,
\qquad p=N^{-3/4},
$$

where the positive constant $c$ will be chosen small, and sample the [binomial random graph](../../../../../../binomial-random-graph.md) $G(N,p)$. If $X$ counts its copies of $C_4$, then

$$
\mathbb EX=3\binom N4p^4\leq\frac N8.
$$

If $Y$ counts its independent $k$-sets, then

$$
\mathbb EY
=\binom Nk(1-p)^{\binom k2}
\leq
\left(\frac{eN}{k}\right)^k
\exp\left(-\frac{pk(k-1)}2\right).
$$

Here $pk\sim c^{-3/4}\log k$. Choosing $c$ sufficiently small makes the negative exponential term dominate $k\log(eN/k)$, so $\mathbb EY=o(1)$. By [Markov inequality](../../../../../../markov-inequality.md), with positive probability $X<N/2$ and $Y=0$.

Starting from such a graph, delete one vertex from each remaining $C_4$. This [random alteration method](../../../../../../random-alteration-method.md) removes fewer than $N/2$ vertices, destroys every $C_4$, and cannot create an [independent set](../../../../../../independent-set-graph-theory.md) of order $k$. The resulting graph has at least $N/2$ vertices, so its edges and nonedges give a red-blue colouring with neither a red $C_4$ nor a blue $K_k$. Consequently

$$
\boxed{R(C_4,K_k)>N/2
\geq c'\left(\frac{k}{\log k}\right)^{4/3}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
