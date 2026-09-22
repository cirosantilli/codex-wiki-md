<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [magnetic energy](../../../../magnetic-energy.md) $E_B=(2\mu_0)^{-1}\int_V|\mathbf B|^2\,dV$. Vary the [Euler potentials](../../../../euler-potentials.md) while keeping their boundary values fixed. The [field variation](../../../../calculus-of-variations-split.md) is

$$
\delta\mathbf B=\nabla\delta\alpha\times\nabla\beta+
\nabla\alpha\times\nabla\delta\beta
=\nabla\times\left(\delta\alpha\nabla\beta-\delta\beta\nabla\alpha\right).
$$

Let $\delta\mathbf A=\delta\alpha\nabla\beta-\delta\beta\nabla\alpha$. [Integration by parts](../../../../integration-by-parts.md) gives

$$
\delta E_B=\frac1{\mu_0}\int_V\delta\mathbf A\cdot(\nabla\times\mathbf B)\,dV,
$$

because $\delta\mathbf A=0$ on the boundary. Therefore

$$
\delta E_B=\frac1{\mu_0}\int_V\left[
\delta\alpha\,\nabla\beta\cdot(\nabla\times\mathbf B)
-\delta\beta\,\nabla\alpha\cdot(\nabla\times\mathbf B)\right]dV.
$$

The two interior [variations](../../../../calculus-of-variations-split.md) are independent. At a smooth [minimum](../../../../local-minimum.md) their coefficients must vanish, so the [curl](../../../../curl.md) is [perpendicular](../../../../orthogonal-vectors.md) to both potential [gradients](../../../../gradient.md) and hence parallel to $\mathbf B$ wherever $\mathbf B\ne0$:

$$
\boxed{\nabla\times\mathbf B=\lambda(\mathbf x)\mathbf B,
\qquad\mathbf J\times\mathbf B=0,
\quad\mathbf J=\frac1{\mu_0}\nabla\times\mathbf B.}
$$

This is a [force-free magnetic field](../../../../force-free-magnetic-field.md): the [Lorentz force density](../../../../lorentz-force-density.md) vanishes. Taking the [divergence](../../../../divergence.md) also gives $\mathbf B\cdot\nabla\lambda=0$, so the proportionality factor is constant along a [field line](../../../../magnetic-field-line.md) but need not be the same on different lines.

The fixed-label [variation](../../../../calculus-of-variations-split.md) preserves the encoded [field-line connection](../../../../magnetic-field-line.md) rather than allowing arbitrary [reconnection](../../../../magnetic-reconnection.md) during minimization. The argument proves a necessary condition for a smooth [minimum](../../../../local-minimum.md), not that every [force-free stationary field](../../../../force-free-magnetic-field.md) is a stable energy [minimum](../../../../local-minimum.md). It also does not include [gas pressure](../../../../pressure-split.md) or [gravity](../../../../gravity.md) in the minimized [functional](../../../../functional.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
