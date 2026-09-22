<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $S=\|\sigma\|_\infty$, $K=\|b\|_\infty$, and write $X_t-x_0=M_t+A_t$, where $M_t=\int_0^t\sigma(X_s)\,dB_s$ and $A_t=\int_0^tb(X_s)\,ds$. The [Itô isometry](../../../../../../ito-isometry.md) and boundedness give

$$
\mathbb E|X_t-x_0|^2\le2S^2t+2K^2t^2\longrightarrow0.
$$

Continuity and boundedness of $b$ then imply $\mathbb E b(X_s)\to b(x_0)$. Since $M$ has mean zero,

$$
\frac{\mathbb EX_t-x_0}{t}=\frac1t\int_0^t\mathbb E b(X_s)\,ds\longrightarrow b(x_0).
$$

For the [variance](../../../../../../variance-split.md), $\mathbb EM_t^2=\int_0^t\mathbb E\sigma(X_s)^2\,ds$. The remaining terms satisfy

$$
\mathbb EA_t^2\le K^2t^2,\qquad |\mathbb E(M_tA_t)|\le SKt^{3/2},\qquad (\mathbb E(X_t-x_0))^2\le K^2t^2.
$$

Continuity of $\sigma$ and the initial $L^2$ convergence give $\mathbb E\sigma(X_s)^2\to\sigma(x_0)^2$. Expanding the [variance](../../../../../../variance-split.md) and dividing by $t$ proves the [initial mean and variance derivatives of an Itô diffusion](../../../../../../initial-mean-and-variance-derivatives-of-an-ito-diffusion.md):

$$
\boxed{\left.\frac d{dt}\mathbb EX_t\right|_{0+}=b(x_0),\qquad\left.\frac d{dt}\operatorname{Var}(X_t)\right|_{0+}=\sigma(x_0)^2.}
$$

The derivatives at the initial time are right derivatives because the process is indexed by $t\ge0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
