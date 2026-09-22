<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With the symmetric Fourier normalization displayed in the question, the [creation and annihilation operators](../../../../../../creation-and-annihilation-operators.md) obey the [canonical commutation relation](../../../../../../canonical-commutation-relation.md)

$$
\boxed{[\hat a_{\mathbf k},\hat a_{\mathbf k'}^\dagger]
=\delta^{(3)}(\mathbf k-\mathbf k')},
\qquad
[\hat a_{\mathbf k},\hat a_{\mathbf k'}]
=[\hat a_{\mathbf k}^\dagger,\hat a_{\mathbf k'}^\dagger]=0.
$$

Since $\delta\hat\phi=\hat f/a$, its vacuum [two-point correlation function](../../../../../../two-point-correlation-function.md) is

$$
\langle0|\delta\hat\phi(\tau,\mathbf x)
\delta\hat\phi(\tau,\mathbf x+\mathbf r)|0\rangle
=\int\frac{d^3k}{(2\pi)^3}
\frac{|f_k(\tau)|^2}{a^2}e^{-i\mathbf k\cdot\mathbf r}.
$$

Comparison with the definition in the question gives

$$
\Delta_{\delta\phi}^2(k,\tau)
=\frac{k^3}{2\pi^2}\frac{|f_k|^2}{a^2}.
$$

Using $|f_k|^2=(1+1/(k^2\tau^2))/(2k)$ and $a=-1/(H\tau)$,

$$
\boxed{\Delta_{\delta\phi}^2(k,\tau)
=\left(\frac H{2\pi}\right)^2(1+k^2\tau^2)}.
$$

On [superhorizon scales](../../../../../../superhorizon-scale.md), $k\ll aH$ or $|k\tau|\ll1$, so the [scale-invariant inflationary power spectrum](../../../../../../scale-invariant-inflationary-power-spectrum.md) freezes to

$$
\boxed{\Delta_{\delta\phi}^2=\left(\frac H{2\pi}\right)^2}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
