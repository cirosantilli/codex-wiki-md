<h1 id="3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use [von Neumann stability analysis](../../../../../../von-neumann-stability-analysis.md) on the infinite grid. For the [Fourier mode](../../../../../../fourier-mode.md) $u_{m,k}=\widehat u(t)e^{i(m\xi+k\eta)}$, the semidiscrete [eigenvalue](../../../../../../eigenvalue.md) is

$$
\lambda_h(\xi,\eta)=\frac1h\left[-\frac32-\frac12e^{-i\xi}+\frac12e^{i\xi}
+2e^{i\eta}-\frac12e^{2i\eta}\right]
=\frac{-(1-\cos\eta)^2+i[\sin\xi+(2-\cos\eta)\sin\eta]}h.
$$

Its real part is nonpositive for every frequency. The mode evolves by $\widehat u(t)=e^{t\lambda_h}\widehat u(0)$, whose modulus does not grow. The [discrete Fourier transform](../../../../../../discrete-fourier-transform.md) and [Parseval identity](../../../../../../parseval-identity.md) therefore yield

$$
\boxed{\|u(t)\|_{\ell_h^2}\le\|u(0)\|_{\ell_h^2}\quad(t\ge0),}
$$

with a bound independent of $h$, where $\|u\|_{\ell_h^2}^2=h^2\sum_{m,k}|u_{m,k}|^2$. Hence **the semidiscrete method is stable**. Frequencies with $\eta=0$ are nondissipative rather than unstable.

The same sign can be seen directly by [summation by parts](../../../../../../abel-s-summation-formula.md): the centred $x$ operator is skew-adjoint, and for the unitary $y$ shift $S_y$,

$$
\operatorname{Re}\langle u,D_{y,+,2}u\rangle_h
=-\frac1{4h}\|(S_y-I)^2u\|_h^2\le0.
$$

This is an energy version of the [dissipative second-order forward advection stencil](../../../../../../dissipative-second-order-forward-advection-stencil.md). A subsequent time integrator would need its own stability condition; semidiscrete stability does not assert that every fully discrete method is stable.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [3](../../3.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
