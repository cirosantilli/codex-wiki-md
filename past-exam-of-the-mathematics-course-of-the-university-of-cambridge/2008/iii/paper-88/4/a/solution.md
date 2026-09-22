<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\psi=e^{ikx}E(x,\mathbf s)$, $\mathbf s=(y,z)$. In the weak-contrast approximation $n^2\simeq1+2\mu W$, neglecting $E_{xx}$ relative to $kE_x$ gives the [parabolic wave equation](../../../../../../parabolic-wave-equation.md)

$$
2ikE_x+\Delta_\perp E+2k^2\mu WE=0,
\qquad E_x=\frac{i}{2k}\Delta_\perp E+ik\mu WE.
$$

For the [mutual coherence](../../../../../../coherence-of-a-normalized-matrix.md) $\Gamma(x;\mathbf s_1,\mathbf s_2)=\mathbb E[E_1E_2^*]$, differentiating gives the exact moment equation within this wave approximation,

$$
\boxed{\Gamma_x=\frac{i}{2k}(\Delta_1-\Delta_2)\Gamma
+ik\mu\,\mathbb E[(W_1-W_2)E_1E_2^*].}
$$

This is an evolution equation but not a closed one. Even a jointly [Gaussian random field](../../../../../../gaussian-random-field.md) does not make $W$ independent of $E$, which depends on its history. Transverse [statistical homogeneity](../../../../../../statistical-homogeneity.md) alone therefore does not close the second moment. A covariance or longitudinal Markov approximation is additional information.

Under the white-in-$x$ assumption introduced in the next part, interpret $W\,dx=d\mathcal B_x$, a [longitudinal Brownian field with transverse covariance](../../../../../../longitudinal-brownian-field-with-transverse-covariance.md) $C$, and use the [Stratonovich integral](../../../../../../stratonovich-integral.md) as the smooth-medium limit. Conversion to the [Itô integral](../../../../../../ito-integral.md) yields

$$
dE=\left(\frac{i}{2k}\Delta_\perp E-\frac12k^2\mu^2C(0)E\right)dx
+ik\mu E\,d\mathcal B_x.
$$

The product rule with quadratic variation gives the closed [mutual coherence in a white-noise parabolic medium](../../../../../../mutual-coherence-in-a-white-noise-parabolic-medium.md) equation,

$$
\boxed{\Gamma_x=\frac{i}{2k}(\Delta_1-\Delta_2)\Gamma
-k^2\mu^2[C(0)-C(\mathbf s_1-\mathbf s_2)]\Gamma.}
$$

The two attenuation drifts contribute $-k^2\mu^2C(0)$ and the cross variation contributes $+k^2\mu^2C(\mathbf s_1-\mathbf s_2)$. The coefficient $C$ is the white-noise covariance intensity; it replaces, rather than literally retains, the original finite pointwise variance of $W$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
