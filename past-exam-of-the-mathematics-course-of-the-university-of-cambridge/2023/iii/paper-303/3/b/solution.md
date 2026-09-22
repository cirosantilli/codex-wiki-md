<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the $O(2)$ model write

$$
\boldsymbol\phi=(v+\rho)(\cos\theta,\sin\theta),
\qquad
v^2=-\frac{\mu^2}{4g}.
$$

At long distances the massive radial field $\rho$ can be neglected, leaving the [Goldstone-mode effective free energy](../../../../../../goldstone-mode-effective-free-energy.md)

$$
F_\theta=\frac{\gamma v^2}{2}\int d^dx\,(\nabla\theta)^2.
$$

Therefore

$$
\langle\theta(\mathbf x)\theta(\mathbf y)\rangle
=\frac1{\gamma v^2}\int\frac{d^dk}{(2\pi)^d}
\frac{e^{-i\mathbf k\cdot(\mathbf x-\mathbf y)}}{k^2}.
$$

The mode is massless, so its [correlation length](../../../../../../correlation-length.md) is infinite. For $d>2$ its large-distance Green function is

$$
\langle\theta(\mathbf x)\theta(\mathbf y)\rangle
\sim\frac{\Gamma(d/2-1)}{4\pi^{d/2}\gamma v^2}\,r^{2-d}.
$$

For $d=2$ it is $-(2\pi\gamma v^2)^{-1}\log(r/a)$ up to an infrared-dependent constant, and in $d=1$ it is $-|r|/(2\gamma v^2)$ up to such a constant.

The invariant diagnostic is the [phase-difference variance](../../../../../../phase-difference-variance.md)

$$
\langle[\theta(\mathbf r)-\theta(0)]^2\rangle
=\frac2{\gamma v^2}\int\frac{d^dk}{(2\pi)^d}
\frac{1-\cos(\mathbf k\cdot\mathbf r)}{k^2}.
$$

It diverges linearly in $d=1$ and logarithmically in $d=2$, destroying true long-range order, but approaches a finite infrared limit for $d=3,4$. Thus the continuous-symmetry ordered phase exists for $d=3,4$ and not for $d=1,2$, in agreement with the [Mermin-Wagner theorem](../../../../../../mermin-wagner-theorem.md). The lower critical dimension is $d_{\mathrm{lc}}=2$; the two-dimensional $O(2)$ model can instead show [quasi-long-range order below a BKT transition](../../../../../../berezinskii-kosterlitz-thouless-transition.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 303](../../../paper-303-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
