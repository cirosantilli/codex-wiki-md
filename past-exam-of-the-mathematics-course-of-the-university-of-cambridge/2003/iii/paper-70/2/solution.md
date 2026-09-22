<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the material-first [nominal stress tensor](../../../../../nominal-stress-tensor.md) convention $N_{\alpha i}$, whose reference-volume power is $N_{\alpha i}\dot A_{i\alpha}$. At a regular constraint point, $F_{,A}\ne0$, all admissible deformation rates satisfy $F_{,A_{i\alpha}}\dot A_{i\alpha}=0$. Equality of mechanical power and the derivative of the [strain energy density](../../../../../strain-energy-density.md) gives

$$
\left(N_{\alpha i}-W_{,A_{i\alpha}}\right)\dot A_{i\alpha}=0
$$

for every [vector](../../../../../vector.md) in this eight-dimensional tangent hyperplane. Its [orthogonal complement](../../../../../orthogonal-complement.md) is the span of $F_{,A}$. Consequently the [constraint reaction in hyperelastic stress](../../../../../constraint-reaction-in-hyperelastic-stress.md) is

$$
\boxed{N_{\alpha i}=W_{,A_{i\alpha}}+qF_{,A_{i\alpha}}.}
$$

The scalar [Lagrange multiplier](../../../../../lagrange-multiplier.md) $q$ is not determined by the work identity: its contribution vanishes on every allowed rate. Regularity matters. For example, replacing a regular [incompressibility](../../../../../incompressible-flow.md) constraint by $(\det A-1)^2=0$ would give zero gradient on the same admissible set and could not represent an arbitrary pressure reaction through that gradient.

For [incompressibility](../../../../../incompressible-flow.md) use the regular function $F=J-1$, with $J=\det A$. Differentiating the alternating-tensor expression for $J$ gives

$$
\frac{\partial J}{\partial A_{i\alpha}}
=\frac12\epsilon_{ijk}\epsilon_{\alpha\beta\gamma}A_{j\beta}A_{k\gamma}
=J(A^{-1})_{\alpha i}.
$$

The first expression is the cofactor entry; contracting it with $A_{j\alpha}$ gives $J\delta_{ij}$, proving the inverse formula. On $J=1$ this yields

$$
\boxed{N_{\alpha i}=W_{,A_{i\alpha}}+q(A^{-1})_{\alpha i}.}
$$

With this plus-sign convention $q$ is the negative of the usual pressure multiplier.

For an equibiaxially stretched sheet, [incompressibility](../../../../../incompressible-flow.md) requires the principal stretches $(\lambda,\lambda,\lambda^{-2})$. The printed sheet expression's $\lambda^{-1/2}$ is inconsistent with this constraint and must be $\lambda^{-2}$; the balloon expression later on the same PDF page has the correct exponent. Let $W_j$ denote the derivative with respect to [principal stretch](../../../../../principal-stretch.md) $\lambda_j$, evaluated on this constrained path. With no applied thickness-direction [traction](../../../../../traction.md),

$$
0=N_{33}=W_3+q\lambda^2,
\qquad q=-\lambda^{-2}W_3.
$$

Isotropy gives $W_1=W_2$ at equal in-plane stretches. Hence

$$
N_{11}=N_{22}=W_1-\lambda^{-3}W_3,
\qquad
\frac d{d\lambda}W(\lambda,\lambda,\lambda^{-2})
=W_1+W_2-2\lambda^{-3}W_3.
$$

The [equibiaxial nominal tension of an incompressible sheet](../../../../../equibiaxial-nominal-tension-of-an-incompressible-sheet.md) is therefore

$$
\boxed{N_{11}=N_{22}=\frac12\frac d{d\lambda}W(\lambda,\lambda,\lambda^{-2}).}
$$

The two equal in-plane nominal tensions do work $2N_{11}\,d\lambda$ per reference volume; the thickness-direction [nominal stress](../../../../../nominal-stress-tensor.md) does no work because it is zero. That is exactly the constrained energy differential, explaining energy conservation. As a check that the printed exponent is a genuine error, a [neo-Hookean solid](../../../../../neo-hookean-solid.md) gives $N=\mu(\lambda-\lambda^{-5})$, zero at the undeformed state. The derivative with the erroneous exponent would instead give $3\mu/4$ at that state.

For the thin spherical balloon, use the leading reference shell volume $4\pi a_0^2h_0$. Its two tangential stretches are $\lambda=a/a_0$, while its thickness stretch is $\lambda^{-2}$ and its current thickness is $h=h_0\lambda^{-2}$. Define $\widehat W(\lambda)=W(\lambda,\lambda,\lambda^{-2})$. Its total [elastic energy](../../../../../elastic-energy.md) at leading thin-shell order is

$$
E=4\pi a_0^2h_0\widehat W(\lambda).
$$

During a quasistatic increment $da$, the enclosed volume changes by $d\mathcal V=4\pi a^2da$, and $d\lambda=da/a_0$. Equating energy change to work of the internal excess pressure gives

$$
p\,4\pi a^2da
=4\pi a_0h_0\widehat W'(\lambda)da,
\qquad
\boxed{p(a)=\frac{h_0}{a_0\lambda^2}\widehat W'(\lambda).}
$$

This is the [inflation pressure of a thin incompressible elastic balloon](../../../../../inflation-pressure-of-a-thin-incompressible-elastic-balloon.md). The approximation neglects through-thickness variation and curvature corrections beyond leading order, and requires $h/a\ll1$. It also agrees with membrane [force](../../../../../force.md) balance: $p=2h\sigma_t/a$, $\sigma_t=\lambda N$, and $N=\widehat W'/2$. Here pressure is [force](../../../../../force.md) per current area, while $N$ is [force](../../../../../force.md) per reference area; confusing them would lose a factor of $\lambda$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
