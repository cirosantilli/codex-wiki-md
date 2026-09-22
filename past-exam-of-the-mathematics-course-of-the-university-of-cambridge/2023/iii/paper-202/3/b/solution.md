<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The exponential process $Z_t=\exp(-B_t-t/2)$ is a martingale. Under the [Girsanov theorem](../../../../../../girsanov-theorem.md) change of measure $d\mathbb Q|_{\mathcal F_t}=Z_t,d\mathbb P|_{\mathcal F_t}$, the process $W_t=B_t+t$ is Brownian motion. Its first hitting time $T_a$ of $a>0$ is finite $\mathbb Q$-almost surely. On $\{T_a\leq t\}$, the [optional sampling theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives

$$
\mathbb Q(T_a\leq t)
=\mathbb E_{\mathbb P}[Z_{T_a}\mathbf1_{\{T_a\leq t\}}]
=e^{-a}\mathbb E_{\mathbb P}
\left[e^{T_a/2}\mathbf1_{\{T_a\leq t\}}\right],
$$

because $B_{T_a}=a-T_a$. Letting $t\to\infty$ and applying the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) yields

$$
\mathbb E e^{T_a/2}=e^a.
$$

This is the [Critical exponential moment of a drifted Brownian hitting time](../../../../../../critical-exponential-moment-of-a-drifted-brownian-hitting-time.md).

## ↑ Ancestors (11)

1. [B](../b.md)
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
