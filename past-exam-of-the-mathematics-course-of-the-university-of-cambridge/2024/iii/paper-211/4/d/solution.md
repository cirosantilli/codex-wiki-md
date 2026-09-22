<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For every stopping time $\tau$, the martingale case of the [optional sampling theorem for a supermartingale](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives $\mathbb EX_\tau=X_0=0$. Hence

$$
\mathbb E(Z_\tau+X_\tau)=\mathbb EZ_\tau.
$$

Use the optimal stopping time from part c and the pathwise inequality

$$
\max_{0\leq t\leq T}(Z_t+X_t)
\geq Z_{\tau^*}+X_{\tau^*}.
$$

Taking expectations gives

$$
\boxed{\mathbb E\max_{0\leq t\leq T}(Z_t+X_t)
\geq\mathbb EZ_{\tau^*}=U_0.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
