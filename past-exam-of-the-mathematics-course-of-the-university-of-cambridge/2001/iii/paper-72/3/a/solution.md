<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Landau-Ginzburg theory](../../../../../../landau-ginzburg-theory.md) describes a slowly varying [order parameter](../../../../../../order-parameter.md) by a local [free-energy functional](../../../../../../free-energy-functional.md) consistent with the microscopic symmetries. For a representative scalar system with spin-inversion symmetry, take the dimensionless functional

$$
\mathcal F[\phi]=\int d^dx\left[\frac c2(\nabla\phi)^2+\frac r2\phi^2+\frac u4\phi^4-h\phi\right],\qquad c,u>0,\quad r=r_0t.
$$

The gradient term penalizes spatial variation, while the even local potential implements the zero-field symmetry $\phi\mapsto-\phi$. The positive quartic coefficient stabilizes a continuous transition. A negative quartic coefficient requires higher powers and can instead produce a [first-order phase transition](../../../../../../first-order-phase-transition.md). A vector [order parameter](../../../../../../order-parameter.md) gives the corresponding rotationally invariant model with powers of $|\boldsymbol\phi|^2$.

In the [mean-field approximation](../../../../../../mean-field-approximation.md), replace the field by a constant $M$ and minimize the local potential. Its equation of state and stable zero-field solutions are

$$
h=rM+uM^3,\qquad
M=0\quad(r>0),\qquad M=\pm\sqrt{-r/u}\quad(r<0).
$$

Below the transition these two minima exhibit [spontaneous symmetry breaking](../../../../../../spontaneous-symmetry-breaking.md). Differentiating the equation of state gives $\chi=(r+3uM^2)^{-1}$: it is $1/r$ above the transition and $1/(2|r|)$ within either ordered phase. At $r=0$, $M=(h/u)^{1/3}$. The minimized zero-field [free-energy density](../../../../../../free-energy-density.md) is zero above and $-r^2/(4u)$ below, apart from an analytic background; its second temperature derivative has a finite jump. Consequently

$$
\boxed{\beta_{\rm MF}=\tfrac12,\quad\gamma_{\rm MF}=1,\quad\delta_{\rm MF}=3,\quad\alpha_{\rm MF}=0.}
$$

To include fluctuations, write $\phi=M+\psi$. The quadratic part is

$$
\mathcal F_2=\frac12\int\frac{d^dq}{(2\pi)^d}\left(cq^2+r+3uM^2\right)|\psi(q)|^2.
$$

A [Gaussian functional integral](../../../../../../gaussian-functional-integral.md) therefore gives $\langle\psi(q)\psi(-q)\rangle=(cq^2+r+3uM^2)^{-1}$, with the momentum-volume delta function understood. The [Ornstein--Zernike correlation function](../../../../../../ornstein-zernike-correlation-function.md) has [correlation length](../../../../../../correlation-length.md) $\xi=\sqrt{c/(r+3uM^2)}$. Thus $\nu_{\rm MF}=1/2$, and at criticality the Gaussian covariance is proportional to $q^{-2}$, giving $\eta_{\rm MF}=0$. Continuous-symmetry ordered phases additionally have transverse [Goldstone modes](../../../../../../goldstone-boson.md), for which the restoring mass vanishes.

The Gaussian integration contributes $\frac12\int d^dq\,(2\pi)^{-d}\log(cq^2+r)$ to the disordered-phase [free-energy density](../../../../../../free-energy-density.md). Differentiating twice with respect to $r$ gives a critical contribution proportional to $\int d^dq\,(cq^2+r)^{-2}$; for $d<4$ its singular part grows as $r^{(d-4)/2}$ and at four dimensions it is logarithmic. Interacting fluctuations thus become important close to the critical point below four dimensions. The [Ginzburg criterion](../../../../../../ginzburg-criterion.md) tests this failure of the [mean-field approximation](../../../../../../mean-field-approximation.md); the [renormalization group](../../../../../../renormalization-group.md) then explains modified exponents and [universality](../../../../../../universality-of-critical-phenomena.md). **Mean-field theory finds the competing minima, while fluctuations determine whether its predicted critical behavior survives at long distance.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
