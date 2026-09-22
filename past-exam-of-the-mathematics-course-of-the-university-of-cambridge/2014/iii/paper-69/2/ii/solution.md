<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Work first with $q$ in the [Schwartz space](../../../../../../schwartz-space.md), so that all Fourier manipulations and spectral [contour integrals](../../../../../../contour-integral.md) are justified; weaker classes follow by the usual density or distribution arguments. Define

$$
E(z,k)=e^{k\bar z-\bar k z},\qquad
Q(k)=\int_{\mathbb C}e^{\bar k\zeta-k\bar\zeta}q(\zeta)\,dA(\zeta).
$$

The phase is purely imaginary. Since $\partial_{\bar z}E=kE$, setting $F=E\Phi$ reduces the spectral equation to $\partial_{\bar z}\Phi=E^{-1}q$. The whole-plane [Cauchy-Pompeiu formula](../../../../../../cauchy-pompeiu-formula.md) therefore constructs the solution decaying spatially at infinity:

$$
\boxed{F(z,k)=\frac{E(z,k)}\pi\int_{\mathbb C}
\frac{e^{\bar k\zeta-k\bar\zeta}q(\zeta)}{z-\zeta}\,dA(\zeta).}
$$

The freedom to add $E$ times an entire function is removed by this decay condition. For every fixed $k$, the integral is a spatial [Cauchy-Green operator](../../../../../../cauchy-green-operator.md) applied to a modulated source.

Now differentiate in the conjugate spectral parameter. The two exponential derivatives produce $\zeta-z$, canceling the Cauchy denominator, so

$$
\boxed{\partial_{\bar k}F(z,k)=-\frac1\pi E(z,k)Q(k).}
$$

This is the spectral [dbar equation](../../../../../../dbar-equation.md): its right-hand side is the forward transform of $q$ multiplied by a known plane wave. Apply the whole-plane [Cauchy-Pompeiu formula](../../../../../../cauchy-pompeiu-formula.md) again, now in $k$:

$$
F(z,k)=-\frac1{\pi^2}\int_{\mathbb C}
\frac{E(z,\ell)Q(\ell)}{k-\ell}\,dA(\ell).
$$

The spatial spectral equation also gives $F(z,k)=-q(z)/k+o(k^{-1})$ as $|k|\to\infty$. One way to justify this is to integrate by parts in the first Cauchy integral: $F=-q/k+T_k(q_{\bar z})/k$, where the modulated Cauchy integral $T_k(q_{\bar z})$ tends to zero by the [Riemann-Lebesgue lemma](../../../../../../riemann-lebesgue-lemma.md). Comparing the $1/k$ coefficient of the spectral [contour integral](../../../../../../contour-integral.md) therefore gives

$$
\boxed{Q(k)=\int_{\mathbb C}e^{\bar k z-k\bar z}q(z)\,dA(z),\qquad
q(z)=\frac1{\pi^2}\int_{\mathbb C}e^{k\bar z-\bar k z}Q(k)\,dA(k).}
$$

This derives the transform pair from two uses of the [Cauchy-Pompeiu formula](../../../../../../cauchy-pompeiu-formula.md), not from an assumed inversion formula.

To identify the usual normalization, write $z=x+iy$ and $k=k_1+ik_2$. Then $\bar kz-k\bar z=2i(k_1y-k_2x)$. Set $\xi_1=2k_2$, $\xi_2=-2k_1$, so $d\xi_1d\xi_2=4\,dA(k)$. The result is exactly the two-dimensional [Fourier transform](../../../../../../fourier-transform.md) pair

$$
\boxed{\widehat q(\xi)=\int_{\mathbb R^2}e^{-i\xi\cdot x}q(x)\,dx,\qquad
q(x)=\frac1{(2\pi)^2}\int_{\mathbb R^2}e^{i\xi\cdot x}\widehat q(\xi)\,d\xi.}
$$

The factor four in the real-frequency change of variables is essential.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
