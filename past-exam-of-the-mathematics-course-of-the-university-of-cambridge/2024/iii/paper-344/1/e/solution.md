<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Translational invariance makes the pointwise [variance](../../../../../../variance-split.md) independent of $\mathbf r$. Applying [Parseval identity](../../../../../../parseval-identity.md) to the stated Fourier convention gives

$$
\sigma^2
=\langle|\phi(\mathbf r)|^2\rangle_0
=\frac1V\sum_{\mathbf q}\langle|\phi_{\mathbf q}|^2\rangle_0
=\frac1V\sum_{\mathbf q}\frac1{J(q)}.
$$

In the [thermodynamic limit](../../../../../../thermodynamic-limit.md), the reciprocal-lattice sum becomes

$$
\sigma^2
=\int\frac{d^d\mathbf q}{(2\pi)^d}\frac1{J(q)}.
$$

At each point $\phi(\mathbf r)$ is a centered [Gaussian random variable](../../../../../../gaussian-random-variable.md), so the supplied absolute third moment gives

$$
\boxed{g\int d^d\mathbf r\,\langle|\phi(\mathbf r)|^3\rangle_0
=\frac{4gV}{\sqrt{2\pi}}\sigma^3
=\frac{4gV}{\sqrt{2\pi}}
\left[
\int\frac{d^d\mathbf q}{(2\pi)^d}\frac1{J(q)}
\right]^{3/2}.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
