<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

An [electromagnetic field tensor](../../../../../../electromagnetic-field-tensor.md) obeys the homogeneous [Maxwell equations](../../../../../../maxwell-equations.md) $dF=0$. Together with its invariance under the [Killing vector field](../../../../../../killing-vector-field.md) $V$, [Cartan's magic formula](../../../../../../cartan-s-magic-formula.md) gives $d(\iota_VF)=\mathcal L_VF-\iota_VdF=0$. The [local potential of a closed differential one-form](../../../../../../local-potential-of-a-closed-differential-one-form.md) construction, the one-form [Poincaré lemma](../../../../../../poincare-lemma.md), therefore supplies a [scalar field](../../../../../../scalar-field.md) $\Phi$ on a sufficiently small [contractible](../../../../../../contractible-space.md) neighborhood with

$$
\boxed{\iota_VF=d\Phi.}
$$

For an explicit local proof, write $\iota_VF=\alpha_i(x)dx^i$ on a coordinate ball centered at zero and take $\Phi(x)=\int_0^1 x^i\alpha_i(sx)\,ds$. Since $d\alpha=0$, differentiating under the integral gives $\partial_j\Phi=\int_0^1[\alpha_j(sx)+s x^i\partial_i\alpha_j(sx)]ds=\alpha_j(x)$. There need not be a global potential when this closed one-form has nonzero periods. The homogeneous Maxwell equation is essential; an arbitrary invariant two-form would not suffice.

Use [proper time](../../../../../../proper-time.md) for the massive particle, let $u$ be its tangent, and assume $m\ne0$. The [Killing equation](../../../../../../killing-equation.md) makes $u^au^b\nabla_aV_b=0$. The [Lorentz force](../../../../../../lorentz-force.md) equation then implies

$$
\frac d{d\tau}(V_au^a)=\frac qm V_aF^a{}_bu^b=\frac qm V^aF_{ab}u^b=\frac qm\frac{d\Phi}{d\tau}.
$$

Consequently the local conserved quantity is

$$
\boxed{mV_au^a-q\Phi=\text{constant}.}
$$

The sign follows from contracting $F$ in its first argument, exactly as in the source. Adding a constant to $\Phi$ merely shifts the conserved quantity. This is a [charged-particle conserved quantity from a Killing symmetry](../../../../../../charged-particle-conserved-quantity-from-a-killing-symmetry.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
