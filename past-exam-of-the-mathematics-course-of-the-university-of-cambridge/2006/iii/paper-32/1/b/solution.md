<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [almost sure supermartingale convergence theorem](../../../../../../almost-sure-supermartingale-convergence-theorem.md) applies to the $L^1$-bounded [supermartingale](../../../../../../supermartingale.md) $X$. Hence $X_n\to X_\infty$ [almost surely](../../../../../../almost-sure-convergence.md), and the [Fatou lemma](../../../../../../fatou-s-lemma.md) gives $\mathbb E|X_\infty|\leq\sup_n\mathbb E|X_n|<\infty$. Take the version of $X_\infty$ obtained from the sequence, so it is measurable for $\mathcal F_\infty=\sigma(\bigcup_n\mathcal F_n)$. Set

$$
M_n=\mathbb E[X_\infty\mid\mathcal F_n],\qquad Y_n=X_n-M_n.
$$

The [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) makes $M$ a [martingale](../../../../../../martingale-split.md), and the [uniform integrability of conditional expectations](../../../../../../uniform-integrability-of-conditional-expectations.md) makes it [uniformly integrable](../../../../../../uniform-integrability.md). Explicitly, with $Z=X_\infty$, $C=\mathbb E|Z|$, and $R,K>0$, we have $|M_n|\leq R+\mathbb E[|Z|\mathbf1_{\{|Z|>R\}}\mid\mathcal F_n]$, so

$$
\mathbb E[|M_n|\mathbf1_{\{|M_n|>K\}}]\leq\frac{RC}{K}+\mathbb E[|Z|\mathbf1_{\{|Z|>R\}}].
$$

First choose $R$ large, then $K$ large. This proves [uniform integrability](../../../../../../uniform-integrability.md) uniformly in $n$.

The [uniformly integrable martingale convergence theorem](../../../../../../uniformly-integrable-martingale-convergence-theorem.md) gives a limit $M_\infty$ both [almost surely](../../../../../../almost-sure-convergence.md) and in $L^1$. For $A\in\mathcal F_j$ and $n\geq j$, $\mathbb E[M_n\mathbf1_A]=\mathbb E[X_\infty\mathbf1_A]$. Passing to the $L^1$ limit and then extending from the algebra $\bigcup_j\mathcal F_j$ to $\mathcal F_\infty$ identifies $M_\infty=X_\infty$ [almost surely](../../../../../../almost-sure-convergence.md). Finally,

$$
\mathbb E[Y_{n+1}\mid\mathcal F_n]=\mathbb E[X_{n+1}\mid\mathcal F_n]-M_n\leq Y_n,
\qquad Y_n=X_n-M_n\longrightarrow0\quad\text{a.s.}
$$

Thus **$X=M+Y$ with $M$ uniformly integrable and $Y$ a supermartingale tending almost surely to zero**. The [terminal decomposition of an L1-bounded supermartingale](../../../../../../terminal-decomposition-of-an-l1-bounded-supermartingale.md) does not require $Y\geq0$ or $Y_n\to0$ in $L^1$. Indeed, for $X$ equal to the negative of the [fair-coin doubling martingale](../../../../../../fair-coin-doubling-martingale.md), $X_\infty=0$, $M=0$, and $Y=X$ is negative and has constant absolute mean one.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
