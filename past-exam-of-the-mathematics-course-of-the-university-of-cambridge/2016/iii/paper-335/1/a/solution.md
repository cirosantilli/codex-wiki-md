<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the time convention $e^{-i\omega t}$. The free-space [Helmholtz equation](../../../../../../helmholtz-equation.md), with $\psi=e^{ikx}E$, gives the exact reduced equation

$$
E_{xx}+2ikE_x+E_{zz}=0.
$$

For a forward [plane wave](../../../../../../plane-wave.md) at angle $\alpha$, $E_x=O(k\alpha^2E)$ and $E_{zz}=O(k^2\alpha^2E)$, whereas $E_{xx}=O(k^2\alpha^4E)$. Thus the [paraxial approximation](../../../../../../paraxial-approximation.md) neglects $E_{xx}$ relative to $2ikE_x$. **The reduced field satisfies the [parabolic wave equation](../../../../../../parabolic-wave-equation.md)**

$$
\boxed{2ikE_x+E_{zz}=0,\qquad E_x=\frac{i}{2k}E_{zz}.}
$$

With the [Fourier transform](../../../../../../fourier-transform.md) convention used below and its inverse, this becomes an [ordinary differential equation](../../../../../../ordinary-differential-equation.md) for each transverse [wavenumber](../../../../../../wavenumber.md):

$$
\partial_x\widehat E(x,\nu)=-\frac{i\nu^2}{2k}\widehat E(x,\nu),\qquad
\boxed{\widehat E(x,\nu)=e^{-i\nu^2x/(2k)}\widehat E(0,\nu).}
$$

Consequently the initial-value solution is

$$
E(x,z)=\int_{\mathbb R}\widehat E(0,\nu)e^{i\nu z-i\nu^2x/(2k)}\,d\nu.
$$

Equivalently, evaluating the oscillatory [Gaussian integral](../../../../../../gaussian-integral.md) gives the [one-dimensional transverse Fresnel propagation](../../../../../../one-dimensional-transverse-fresnel-propagation.md) formula

$$
\boxed{E(x,z)=\sqrt{\frac{k}{2\pi ix}}\int_{\mathbb R}
\exp\!\left(\frac{ik(z-z')^2}{2x}\right)E(0,z')\,dz',\qquad x>0.}
$$

The square-root branch has $\sqrt{1/i}=e^{-i\pi/4}$. The formula is an [oscillatory integral](../../../../../../oscillatory-integral.md) for general data, or the [Fresnel propagator](../../../../../../fresnel-propagator.md) acting on [square-integrable functions](../../../../../../square-integrable-function.md). It approaches the initial field as $x\downarrow0$. A [plane wave](../../../../../../plane-wave.md) has transverse [wavenumber](../../../../../../wavenumber.md) $\nu=k\sin\alpha$; the reduced axial phase $-\nu^2x/(2k)$ agrees with $k(\cos\alpha-1)x$ through order $\alpha^2$. This also checks the sign. The [paraxial approximation](../../../../../../paraxial-approximation.md) applies to $|\nu|\ll k$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
