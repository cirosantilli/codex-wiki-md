<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

In this static scalar problem, a [classical field-theory soliton](../../../../../classical-field-theory-soliton-split.md) is a nontrivial smooth localized finite-energy field configuration which is static in its rest frame and stable against admissible small perturbations. Moving examples are obtained by a [Lorentz boost](../../../../../lorentz-boost.md). The relevant static energy is

$$
E[\phi]=T+V,\qquad T=\frac12\int_{\mathbb R^D}|\nabla\phi|^2\,d^Dx,\qquad V=\int_{\mathbb R^D}U(\phi)\,d^Dx.
$$

Use the usual vacuum normalization $U\geq0$, with zero energy at a vacuum, and impose finite-energy vacuum behavior at spatial infinity. These assumptions, together with the unconstrained real target and the canonical two-derivative kinetic term, are the hypotheses of the following [Derrick theorem](../../../../../derrick-s-theorem.md) argument.

For [Derrick scaling](../../../../../derrick-scaling.md) $\phi_\lambda(x)=\phi(\lambda x)$, change variables to obtain

$$
E(\lambda)=\lambda^{2-D}T+\lambda^{-D}V.
$$

A static solution must be stationary under this admissible scale variation. The [Derrick virial identity](../../../../../derrick-virial-identity.md) is

$$
(2-D)T-DV=0.
$$

For $D>2$, both terms are nonpositive and the gradient term is strictly negative for a nonconstant field, so no nontrivial static solution is possible. At $D=2$, the identity forces $V=0$, but the gradient term is scale invariant and a further argument is needed.

Since $U\geq0$, $V=0$ implies $U(\phi(x))=0$ everywhere. Every zero of a differentiable nonnegative potential has $U'=0$. The static [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) $\Delta\phi=U'(\phi)$ therefore makes $\phi$ a [harmonic function](../../../../../harmonic-function.md). Each derivative $\partial_i\phi$ is harmonic and belongs to [L2 space](../../../../../l2-space-is-a-hilbert-space.md) by finite energy. Its mean-value property and the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) on a ball of radius $R$ imply

$$
|\partial_i\phi(x)|^2\leq\frac1{\operatorname{vol}B_R}\int_{B_R(x)}|\partial_i\phi|^2\,d^Dy\leq\frac{2T}{\operatorname{vol}B_R}.
$$

Letting $R\to\infty$ gives $\partial_i\phi=0$. This proves the [two-dimensional flat-target Derrick obstruction](../../../../../two-dimensional-flat-target-derrick-obstruction.md). Thus **a nontrivial static real-scalar soliton in this class can occur only for $D=1$**. The argument does not apply unchanged to curved-target sigma models or gauge-field energies.

In one dimension the scale identity is $T=V$, and the second scale derivative is $2V>0$ for a nontrivial solution; scale variation does not rule it out. To derive the [Bogomolny equations](../../../../../bogomolny-equations.md), write $U=\tfrac12W'(\phi)^2$ on the field interval of interest. [Completing the square](../../../../../completing-the-square.md) gives

$$
E=\frac12\int_{-\infty}^{\infty}(\phi'\mp W')^2\,dx\pm[W(\phi(+\infty))-W(\phi(-\infty))].
$$

Therefore the [Bogomolny bound](../../../../../bogomolny-bound.md) and its saturation equation are

$$
\boxed{E\geq|\Delta W|,\qquad\phi'=\pm W'(\phi).}
$$

Equivalently, for a monotone field connecting adjacent vacua, $\phi'=\pm\sqrt{2U(\phi)}$, with the sign chosen for its direction. Differentiating the first-order equation gives $\phi''=W'W''=U'$, verifying the static [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md). Saturation minimizes energy within the fixed-boundary [topological sector](../../../../../topological-sector.md).

For the given sextic potential, factorization gives $U(\phi)=\phi^2(\phi^2-4)^2$, so the vacua are $-2,0,2$. Choose

$$
W'(\phi)=\sqrt2\,\phi(4-\phi^2),\qquad W(\phi)=\sqrt2\left(2\phi^2-\frac{\phi^4}{4}\right).
$$

This choice satisfies $U=W'^2/2$. On $0<\phi<2$, the increasing [kink in a phi-six model](../../../../../kink-in-a-phi-six-model.md) satisfies $\phi'=\sqrt2\phi(4-\phi^2)$. Setting $y=\phi^2$ gives $y'=2\sqrt2\,y(4-y)$. Separation gives

$$
\log\frac{y}{4-y}=8\sqrt2(x-x_0),
$$

and hence

$$
\boxed{\phi_{0\to2}(x)=\frac2{\sqrt{1+e^{-8\sqrt2(x-x_0)}}},\qquad E=4\sqrt2.}
$$

The endpoints are zero and two, and the mass follows from $W(2)-W(0)=4\sqrt2$. The other increasing elementary [scalar-field kink](../../../../../scalar-field-kink.md) is

$$
\boxed{\phi_{-2\to0}(x)=-\frac2{\sqrt{1+e^{8\sqrt2(x-x_0)}}},\qquad E=4\sqrt2.}
$$

It uses the opposite sign of $W'$ and has the same mass. Reflecting $x-x_0$ yields the two decreasing [antikinks](../../../../../antikink.md); $x_0$ is the free center.

There is no single finite-width static kink directly connecting $-2$ to $2$. Multiplying the static equation by $\phi'$ gives the first integral $\phi'^2/2-U=0$ for a finite-energy vacuum-to-vacuum solution. At the intermediate vacuum $\phi=0$, this forces $\phi'=0$. Uniqueness for the smooth second-order field equation makes data $(\phi,\phi')=(0,0)$ stay at that vacuum, so a nontrivial solution cannot cross it at finite $x$. This is the [intermediate-vacuum obstruction to a kink](../../../../../intermediate-vacuum-obstruction-to-a-kink.md); the two elementary transitions can only separate by an infinite interval.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
