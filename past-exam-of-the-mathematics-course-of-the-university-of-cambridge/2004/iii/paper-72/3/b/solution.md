<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a static base state under [dead loading](../../../../../../dead-loading.md), put $v_i=u_i(\xi)e^{i\omega t}$ and take zero incremental [body force](../../../../../../body-force.md) and [traction](../../../../../../traction.md). The admissible squared frequencies are the [eigenvalues](../../../../../../eigenvalue.md) of the weighted [boundary value problem](../../../../../../boundary-value-problem.md)

$$
-(c_{\alpha i\beta j}u_{j,\beta})_{,\alpha}=\rho_0\omega^2u_i\quad\text{in }\Omega_0,\qquad \nu_\alpha c_{\alpha i\beta j}u_{j,\beta}=0\quad\text{on }\partial\Omega_0.
$$

Multiply by $\overline{u_i}$ and integrate over the reference body. The boundary term in [integration by parts](../../../../../../integration-by-parts.md) vanishes, giving the [elastic normal-mode energy identity](../../../../../../elastic-normal-mode-energy-identity.md)

$$
\boxed{\omega^2=\frac{\displaystyle\int_{\Omega_0}\overline{u_{i,\alpha}}c_{\alpha i\beta j}u_{j,\beta}\,dV}{\displaystyle\int_{\Omega_0}\rho_0\overline{u_i}u_i\,dV}.}
$$

For a nonzero mode and positive [mass density](../../../../../../density.md), the denominator is real and positive. The numerator is real by major symmetry of the [incremental elastic moduli](../../../../../../incremental-elastic-moduli.md). Explicitly, if $u=p+iq$ with real $p,q$, the two imaginary cross terms cancel, leaving the sum of the quadratic energies of $\nabla p$ and $\nabla q$. Consequently **every admissible $\omega^2$ is real**. A negative value, when allowed by indefinite moduli, corresponds to exponential growth or decay rather than an oscillation with real frequency.

If the moduli quadratic form is strictly positive on every nonzero real matrix, that same decomposition shows that the numerator is positive whenever $\nabla u$ is nonzero. Thus **$\omega^2>0$ for every nontranslation mode**. Under the usual assumptions of a bounded connected body, regular coefficients and uniform positivity, the [Rayleigh quotient](../../../../../../rayleigh-quotient.md) defines a [self-adjoint operator](../../../../../../self-adjoint-operator.md) with discrete positive squared frequencies on the mass-weighted mean-zero displacement space. Its eigenfunctions give the nontrivial small harmonic oscillations.

There is an unavoidable zero-frequency qualification for the pure [traction](../../../../../../traction.md) problem as printed: $u_i=b_i$, for any nonzero constant vector $b$, has zero gradient, zero incremental [nominal stress](../../../../../../nominal-stress-tensor.md) and $\omega^2=0$. These three constant translations obey all the homogeneous incremental boundary conditions. Under the strict quadratic-form hypothesis they are the entire zero eigenspace on a connected body. Therefore the unrestricted conclusion is

$$
\boxed{\omega^2\ge0;\quad \omega^2=0\text{ precisely for translations}.}
$$

Strict positivity for every nonzero displacement requires excluding these modes, for example by imposing $\int_{\Omega_0}\rho_0u\,dV=0$, or by adding a displacement constraint. If harmonic perturbations are defined to have nonzero frequency from the outset, the requested positivity holds for all those perturbations.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
