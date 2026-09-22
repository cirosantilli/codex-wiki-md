<h1 id="16b/solution">Solution</h1>

↑ **Parent:** [16B](../16b.md)

For a one-dimensional [wavefunction](../../../../../wave-function.md), the [probability density](../../../../../probability-density.md) and [probability current](../../../../../probability-current.md) are

$$
\rho=|\psi|^2,\qquad j=\frac{\hbar}{2mi}\left(\psi^*\psi_x-\psi\psi_x^*\right)=\frac\hbar m\operatorname{Im}(\psi^*\psi_x).
$$

The [Time-dependent Schrödinger equation](../../../../../time-dependent-schrodinger-equation.md) with a real potential is $i\hbar\psi_t=-\hbar^2\psi_{xx}/(2m)+V\psi$. Multiply it and its [complex conjugate](../../../../../complex-conjugate.md) by $\psi^*$ and $\psi$, respectively. Subtracting cancels the real-potential terms and gives

$$
\rho_t=\frac{i\hbar}{2m}(\psi^*\psi_{xx}-\psi\psi_{xx}^*)=-j_x.
$$

This derives the [continuity equation](../../../../../continuity-equation.md) $\rho_t+j_x=0$.

For $k>0$, the specified free-region [wavefunction](../../../../../wave-function.md) combines a right-moving incoming wave of unit amplitude and a left-moving reflected wave with complex reflection amplitude $R$. Applying the free Schrödinger operator to either plane wave gives $E=\hbar^2k^2/(2m)$. Its time factor has modulus one, so

$$
\rho=1+|R|^2+2\operatorname{Re}(Re^{-2ikx}),\qquad \rho_t=0,\qquad j=\frac{\hbar k}{m}(1-|R|^2).
$$

The density includes the stationary interference pattern; $|R|^2$, rather than $R$, is the reflection probability.

For the [finite square well](../../../../../finite-square-well.md), let $k=\sqrt{2mE}/\hbar$ outside and $q=\sqrt{2m(E+V_0)}/\hbar$ inside. Write the stationary parts as $e^{ikx}+Re^{-ikx}$ to the left, $Ae^{iqx}+Be^{-iqx}$ inside, and $Te^{ikx}$ to the right. At both finite potential steps, the [wavefunction](../../../../../wave-function.md) and its first spatial [derivative](../../../../../derivative.md) are continuous. Integrating the stationary [Schrödinger equation](../../../../../schrodinger-equation.md) across a shrinking step proves derivative continuity; a jump of the [wavefunction](../../../../../wave-function.md) would create an unmatched distributional derivative and is excluded.

Propagate the boundary values at $a$ back through the well. The values at zero are

$$
\chi(0)=Te^{ika}\left(\cos qa-i\frac kq\sin qa\right),\qquad
\chi'(0)=Te^{ika}\left(q\sin qa+ik\cos qa\right).
$$

Matching them to $1+R$ and $ik(1-R)$, and adding the two equations after division of the second by $ik$, gives

$$
2=Te^{ika}\left[2\cos qa-i\left(\frac kq+\frac qk\right)\sin qa\right].
$$

Since the exterior wave numbers agree, the [transmission probability](../../../../../transmission-probability.md) is the current ratio $|T|^2$, so

$$
|T|^2=\left[1+\frac{(q^2-k^2)^2}{4k^2q^2}\sin^2qa\right]^{-1}.
$$

When $V_0=3E$, $q=2k=\sqrt{8mE}/\hbar$, yielding

$$
\boxed{|T|^2=\left[1+\frac9{16}\sin^2\frac{a\sqrt{8mE}}{\hbar}\right]^{-1}.}
$$

Classically an incoming particle of positive energy crosses the attractive well and emerges with its original energy, so transmission is one. The quantum result agrees exactly when $qa$ is an integer multiple of $\pi$:

$$
\boxed{a=\frac{n\pi\hbar}{\sqrt{8mE}},\qquad n=1,2,\ldots.}
$$

These are widths with [resonant transmission through a square well](../../../../../resonant-transmission-through-a-square-well.md); the degenerate width zero also has unit transmission.

## ↑ Ancestors (10)

1. [16B](../16b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
