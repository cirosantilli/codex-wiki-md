<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [creation and annihilation operators](../../../../../../creation-and-annihilation-operators.md) obey the canonical bosonic commutation relations

$$
\boxed{[\hat a_{\mathbf k},\hat a^\dagger_{\mathbf k'}]
=(2\pi)^3\delta^{(3)}(\mathbf k-\mathbf k')},
$$



$$
\boxed{[\hat a_{\mathbf k},\hat a_{\mathbf k'}]
=[\hat a^\dagger_{\mathbf k},\hat a^\dagger_{\mathbf k'}]=0},
\qquad \hat a_{\mathbf k}|0\rangle=0.
$$

Since $\delta\phi=\hat f/a$, the vacuum [two-point correlation function](../../../../../../two-point-correlation-function.md) is

$$
\langle0|\delta\phi(\tau,\mathbf x)
\delta\phi(\tau,\mathbf x+\mathbf r)|0\rangle
=\frac1{a^2}\int\frac{d^3k}{(2\pi)^3}|f_k(\tau)|^2e^{-i\mathbf k\cdot\mathbf r}.
$$

For

$$
f_k=\frac{e^{-ik\tau}}{\sqrt{2k}}
\left(1-\frac{i}{k\tau}\right),
$$

one has $|f_k|^2=(1+1/(k^2\tau^2))/(2k)$. Comparison with the definition of the dimensionless [power spectrum](../../../../../../power-spectrum.md) gives

$$
\Delta_{\delta\phi}^2
=\frac{k^3}{2\pi^2a^2}|f_k|^2
=\frac{H^2}{4\pi^2}(1+k^2\tau^2),
$$

where $a=-1/(H\tau)$. On [superhorizon scales](../../../../../../superhorizon-scale.md), $k\ll aH$ or $|k\tau|\ll1$, and therefore

$$
\boxed{\Delta_{\delta\phi}^2=\left(\frac{H}{2\pi}\right)^2}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
