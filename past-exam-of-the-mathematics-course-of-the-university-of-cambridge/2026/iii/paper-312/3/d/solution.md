<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write the matter density as a sum over normalized halo profiles,

$$
\rho(\mathbf x)=\sum_iM_i u(\mathbf x-\mathbf x_i|M_i),
\qquad
\int d^3x\,u(\mathbf x|M)=1.
$$

For $\mathbf k\ne0$, its density contrast is

$$
\delta(\mathbf k)=\frac1{\bar\rho}
\sum_iM_i\widetilde u(k|M_i)e^{-i\mathbf k\cdot\mathbf x_i}.
$$

If halo locations form an uncorrelated Poisson process, only equal-halo terms survive after subtracting the homogeneous contribution. Replacing the sum per unit volume by the halo abundance gives the [one-halo term](../../../../../../one-halo-term.md)

$$
\boxed{P(k)=P_{1h}(k)
=\int_0^\infty dM\,\frac{dn}{dM}
\left(\frac{M}{\bar\rho}\right)^2
|\widetilde u(k|M)|^2}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
