<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $q(x)=\sigma(x)^2p(x)$. The explicit density formula and local integrability assumption give

$$
q(x)=C\exp\left(\int_0^x\frac{2b(s)}{\sigma(s)^2}\,ds\right),\qquad q'(x)=2b(x)p(x).
$$

Hence its [Fokker-Planck probability current](../../../../../../fokker-planck-probability-current.md) $bp-q'/2$ is zero. The stationary adjoint equation is $L^*p=-(bp)'+q''/2=0$. We prove the required integral identity with cutoffs, avoiding an unstated boundary condition on derivatives of $u$.

Choose smooth $0\leq\chi_R\leq1$, equal to one on $[-R,R]$, supported in $[-2R,2R]$, with $|\chi_R'|\leq C_1/R$ and $|\chi_R''|\leq C_2/R^2$. Since $pLu=(qu_x)'/2$, integrate the backward equation in time and integrate by parts twice in space:

$$
\int\chi_Rp\,[u(t,\cdot)-f],dx
=\frac12\int_0^t\int u(s,x)[\chi_R''(x)q(x)+\chi_R'(x)q'(x)]\,dx\,ds.
$$

These integrations have compact support, as permitted in the question. Bounded coefficients and normalized $p$ give

$$
\|q\|_1\leq\|\sigma\|_\infty^2,\qquad\|q'\|_1\leq2\|b\|_\infty.
$$

The right side is bounded in absolute value by

$$
\frac{t\|u\|_\infty}{2}\left(\frac{C_2\|q\|_1}{R^2}+\frac{C_1\|q'\|_1}{R}\right),
$$

which tends to zero. [Dominated convergence](../../../../../../dominated-convergence-theorem.md) on the left therefore proves

$$
\boxed{\int_{\mathbb R}u(t,x)p(x)\,dx=\int_{\mathbb R}f(x)p(x)\,dx.}
$$

This is the [cutoff proof of invariance for a zero-flux diffusion density](../../../../../../cutoff-proof-of-invariance-for-a-zero-flux-diffusion-density.md). In particular, if an independent initial state has density $p$, part (a) and Fubini give a constant expectation of this test function at every time. This consequence alone is sufficient for the final coupling argument.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
