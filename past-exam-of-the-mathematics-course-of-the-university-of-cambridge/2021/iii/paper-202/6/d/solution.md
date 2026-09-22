<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $X$ be a positive strict local martingale solving

$$
dX_t=X_t^2dW_t,
$$

and fix $T>0$. Use the bank account $S^0=1$ and two risky assets

$$
S_t^1=X_t,
\qquad
S_t^2=\mathbb E[X_T\mid\mathcal F_t],
\qquad0\leq t\leq T.
$$

Both discounted prices are nonnegative local martingales under the physical measure itself, so the same supermartingale argument as in part c rules out arbitrage. At maturity,

$$
S_T^1=X_T=S_T^2.
$$

But strictness means $\mathbb E[X_T\mid\mathcal F_t]<X_t$ for some earlier $t$ on a set of positive probability, so the two prices are not indistinguishable before $T$. This no-arbitrage market violates the Law of One Price.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
