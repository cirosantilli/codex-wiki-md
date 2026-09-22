<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $z=z_c+\eta$, with $\eta(0)=\eta(T)=0$. Independent variations of $z$ and $z^*$ give the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) $\ddot z_c+\omega^2z_c=0$. Away from $\sin\omega T=0$ its unique endpoint solution is

$$
z_c(t)=\frac{z_i\sin\omega(T-t)+z_f\sin\omega t}{\sin\omega T}.
$$

[Integration by parts](../../../../../integration-by-parts.md) cancels the linear fluctuation terms and gives $S[z]=S[z_c]+\int_0^T\eta^*\Delta_\omega\eta\,dt$. On the [classical solution](../../../../../classical-solution.md), the [action](../../../../../action.md) is the boundary term $[z_c^*\dot z_c]_0^T$. Substituting the endpoint derivatives therefore gives

$$
S[z_c]=\frac{\omega}{\sin\omega T}\bigl[(|z_f|^2+|z_i|^2)\cos\omega T-z_f^*z_i-z_i^*z_f\bigr].
$$

The remaining [Gaussian path integral](../../../../../gaussian-path-integral.md) contains two real fluctuation coordinates per mode, so it contributes an inverse [functional determinant](../../../../../functional-determinant.md), rather than its inverse square root. Thus $K=e^{iS[z_c]}/\det\Delta_\omega$, with the measure normalization fixing the otherwise arbitrary constant.

For [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md), the normalized sine modes have [eigenvalues](../../../../../eigenvalue.md) $\lambda_j=(\pi j/T)^2-\omega^2$, $j\ge1$. Their [determinant](../../../../../determinant.md) ratio is the convergent [Dirichlet oscillator determinant ratio](../../../../../dirichlet-oscillator-determinant-ratio.md)

$$
\frac{\det\Delta_\omega}{\det\Delta_0}
=\prod_{j\ge1}\left(1-\frac{\omega^2T^2}{\pi^2j^2}\right)
=\frac{\sin\omega T}{\omega T}.
$$

The last equality is the [sine infinite product](../../../../../sine-infinite-product.md). With the prescribed free [determinant](../../../../../determinant.md) this gives

$$
\boxed{\det\Delta_\omega=\frac{\pi i\sin\omega T}{\omega},\qquad K(z_f,z_i;T)=\frac{\omega}{\pi i\sin\omega T}e^{iS[z_c]}.}
$$

The kernel uses the [Feynman i-epsilon prescription](../../../../../feynman-i-epsilon-prescription.md); at a caustic it is a distributional limit, not an ordinary finite function. Its $\omega\to0$ limit is $(\pi iT)^{-1}\exp(i|z_f-z_i|^2/T)$.

There is a sign error in the printed complex-integral hint. For a positive damping parameter $\alpha$, polar integration gives the [regulated complex Fresnel integral](../../../../../regulated-complex-fresnel-integral.md)

$$
\int_{\mathbb C}e^{(i\lambda-\alpha)|z|^2}\,d^2z=\frac{\pi}{\alpha-i\lambda}\longrightarrow\frac{i\pi}{\lambda}=-\frac{\pi}{i\lambda}.
$$

This regulated value, together with the stated free-kernel normalization, fixes the phase consistently.

For $\omega>0$ and positive imaginary-time length $\beta$, [Wick rotation](../../../../../wick-rotation.md) gives

$$
K_E(z_f,z_i;\beta)=\frac{\omega}{\pi\sinh\omega\beta}\exp\left[-\frac{\omega}{\sinh\omega\beta}\bigl((|z_f|^2+|z_i|^2)\cosh\omega\beta-z_f^*z_i-z_i^*z_f\bigr)\right].
$$

Put $z_f=sz_i$ with $s=\pm1$ and use the convergent real [Gaussian integral](../../../../../gaussian-integral.md). Writing $r=e^{-\omega\beta}$ gives

$$
\int d^2z\,K_E(sz,z;\beta)=\frac1{2(\cosh\omega\beta-s)}=\frac r{(1-sr)^2}=\sum_{n\ge1}s^{n-1}nr^n.
$$

This is the [parity-twisted oscillator thermal trace](../../../../../parity-twisted-oscillator-thermal-trace.md). The complex coordinate describes two independent real [quantum harmonic oscillators](../../../../../quantum-harmonic-oscillator.md), each with mass two in these units. Their total energy is $E=\omega(n_x+n_y+1)$; level $n\omega$ has degeneracy $n$, and spatial inversion has [parity operator](../../../../../parity-operator.md) [eigenvalue](../../../../../eigenvalue.md) $(-1)^{n_x+n_y}=(-1)^{n-1}$. The plus sign is $\operatorname{Tr}e^{-\beta H}$; the minus sign is $\operatorname{Tr}(Pe^{-\beta H})$. The alternating [trace](../../../../../matrix-trace.md) inserts parity into a bosonic system; it does not change the oscillators into fermions.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
