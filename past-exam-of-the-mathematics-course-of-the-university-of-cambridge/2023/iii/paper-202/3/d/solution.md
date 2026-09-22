<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $A_t=[M]_t$ and use the [Dambis-Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md) to write $M_t=B_{A_t}$, enlarging the space if necessary after the terminal clock value. In the time-changed filtration, $A_t$ is a stopping time. For $b<0$, let $S_b=\inf\{s:B_s-s=b\}$. Applying part c with $R=A_t$ gives

$$
1=\mathbb E\!\left[
\mathbf1_{\{S_b\leq A_t\}}e^{b+S_b/2}
+\mathbf1_{\{A_t<S_b\}}e^{M_t-A_t/2}
\right].
$$

On $\{S_b\leq A_t\}$, the first integrand is at most $e^be^{A_t/2}$. The assumed [Novikov condition](../../../../../../novikov-s-condition.md) therefore implies

$$
\mathbb E\left[
\mathbf1_{\{S_b\leq A_t\}}e^{b+S_b/2}
\right]
\leq e^b\mathbb E e^{[M]_T/2}\longrightarrow0
$$

as $b\to-\infty$, uniformly for $t\leq T$. Meanwhile $mathbf1_{\{A_t<S_b\}}\uparrow1$, so the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) gives $\mathbb E\mathcal E(M)_t=1$. A nonnegative local martingale with constant expectation is a martingale. Thus $\mathcal E(M^T)$ is a martingale, proving the [Novikov condition](../../../../../../novikov-s-condition.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
