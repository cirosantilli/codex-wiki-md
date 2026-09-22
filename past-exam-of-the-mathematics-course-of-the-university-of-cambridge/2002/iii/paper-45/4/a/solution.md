<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\delta(\mathbf x)$ be a mean-zero [density contrast](../../../../../../density-contrast.md). For a statistically homogeneous and isotropic field, its [two-point correlation function](../../../../../../two-point-correlation-function.md) is $\xi(r)=\langle\delta(\mathbf x)\delta(\mathbf x+\mathbf r)\rangle$, depending only on $r=|\mathbf r|$. For a galaxy point process the corresponding distinct-pair definition is $dP_{12}=\bar n^2[1+\xi(r)]dV_1dV_2$, the excess pair probability relative to independent uniform positions. Self-pair shot noise is separated when using the density-field version.

Specify the Fourier convention by

$$
\delta(\mathbf x)=\int\frac{d^3k}{(2\pi)^3}\delta(\mathbf k)e^{i\mathbf k\cdot\mathbf x},\qquad
\langle\delta(\mathbf k)\delta^*(\mathbf k')\rangle=(2\pi)^3\delta_D^{(3)}(\mathbf k-\mathbf k')P(k).
$$

The diagonal covariance follows from [statistical homogeneity](../../../../../../statistical-homogeneity.md), and isotropy makes the [matter power spectrum](../../../../../../matter-power-spectrum.md) a function of $k$ alone. Substitute the inverse transforms into the correlation and integrate the delta function:

$$
\xi(r)=\int\frac{d^3k}{(2\pi)^3}P(k)e^{i\mathbf k\cdot\mathbf r}.
$$

Choose the polar axis parallel to $\mathbf r$. Angular integration gives $\int d\Omega_k e^{ikr\cos\theta}=4\pi\sin(kr)/(kr)$. Hence

$$
\boxed{\xi(r)=\frac1{2\pi^2}\int_0^\infty k^2P(k)\frac{\sin(kr)}{kr}\,dk.}
$$

Conversely, when the transform is defined, $P(k)=4\pi\int_0^\infty r^2\xi(r)\sin(kr)/(kr)\,dr$. The stated convention fixes every $2\pi$ factor.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
