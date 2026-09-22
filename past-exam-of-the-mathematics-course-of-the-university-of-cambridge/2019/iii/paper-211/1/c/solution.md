<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We prove the contrapositive. Let

$$
N=\{h\in\mathbb R^n:h\cdot X=0\text{ almost surely}\}.
$$

The function $F$ is constant along $N$, so minimize it on $N^\perp$. Suppose there is no $H$ with $H\cdot X\geq0$ almost surely and strict inequality with positive probability. If a sequence $h_k\in N^\perp$ satisfies $\|h_k\|\to\infty$, pass to a subsequence with

$$
\frac{h_k}{\|h_k\|}\longrightarrow H\in N^\perp,
\qquad\|H\|=1.
$$

Because $H\notin N$ and there is no arbitrage direction, $\mathbb P(H\cdot X<0)>0$. On that event, $e^{-h_k\cdot X}\zeta\to\infty$, and [Fatou lemma](../../../../../../fatou-s-lemma.md) gives $\liminf_kF(h_k)=\infty$. Hence every finite sublevel set of $F$ in $N^\perp$ is bounded. It is also closed, so $F$ attains its infimum there and has a bounded minimizing sequence. This contradicts the assumption. Therefore there is a unit vector $H$ satisfying

$$
\boxed{H\cdot X\geq0\text{ almost surely},
\qquad\mathbb P(H\cdot X>0)>0.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
