<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

The [Bolzano-Weierstrass theorem](../../../../../bolzano-weierstrass-theorem.md) in $\mathbb R$ says that every bounded real sequence has a convergent subsequence. For a bounded sequence in $\mathbb R^n$, successively extract subsequences on which the first, second, and so on through the $n$th coordinate converge. The final diagonal subsequence converges in [Euclidean space](../../../../../euclidean-norm.md), proving the theorem in $\mathbb R^n$.

Put $K=D\setminus\bigcup_{z\in S}B_\varepsilon(z)$. Suppose the asserted $\delta$ did not exist. Then there would be $x_k\in D$ and $y_k\in K$ with $\|x_k-y_k\|<1/k$ but $|f(x_k)-f(y_k)|\geq\varepsilon$. Since $K$ is closed and bounded, Bolzano-Weierstrass gives a subsequence $y_k\to y\in K$, and then $x_k\to y$. The point $y$ is not in $S$, because otherwise $y\in B_\varepsilon(y)$, so $f$ has [continuity](../../../../../continuous-function.md) at $y$. Both $f(x_k)$ and $f(y_k)$ tend to $f(y)$, a contradiction. Hence the required **uniform $\delta>0$ exists**.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
