<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

At this critical coupling, construct solutions of the [Bogomolny vortex equations](../../../../../../bogomolny-vortex-equation.md) rather than superpose isolated vortices, which would not respect the nonlinear field equations. Define $D_j=\partial_j-iA_j$ and $j_k=\operatorname{Im}(\overline\Phi D_k\Phi)$. Direct differentiation using $[D_1,D_2]\Phi=-iB\Phi$ gives

$$
|D\Phi|^2=|(D_1+iD_2)\Phi|^2+B|\Phi|^2+\partial_1j_2-\partial_2j_1.
$$

Integrating the last divergence away under the usual finite-energy vortex boundary conditions and completing the magnetic square yields

$$
V=\int\left[|(D_1+iD_2)\Phi|^2+\left(B-\frac{1-|\Phi|^2}{2}\right)^2\right]d^2x+\int B\,d^2x.
$$

Thus positive vortices saturate this [Bogomolny bound](../../../../../../bogomolny-bound.md) when

$$
\boxed{(D_1+iD_2)\Phi=0,\qquad B=\frac{1-|\Phi|^2}{2}.}
$$

Such fields solve the static second-order equations: under any compactly supported variation the flux is unchanged, and the first variation of both zero squares vanishes. The bound here is $2\pi N$, twice the bound in the frequently used half-normalized [Abelian Higgs model](../../../../../../abelian-higgs-model.md) energy.

For the [prescribed-zero construction of planar Abelian Higgs vortices](../../../../../../prescribed-zero-construction-of-planar-abelian-higgs-vortices.md), choose arbitrary points $z_a\in\mathbb C$ and positive integer multiplicities $m_a$, permitting coincident vortices. Away from the zeros, write $\Phi=e^{h/2+i\chi}$, where $h=\log|\Phi|^2$. The first [Bogomolny vortex equation](../../../../../../bogomolny-vortex-equation.md) gives

$$
A_1=\partial_1\chi+\frac12\partial_2h,\qquad
A_2=\partial_2\chi-\frac12\partial_1h.
$$

Choose the phase winding $\chi=\sum_am_a\arg(z-z_a)$ locally. Distributionally its curl contributes $2\pi\sum_am_a\delta_{z_a}$, so the second [Bogomolny vortex equation](../../../../../../bogomolny-vortex-equation.md) becomes the [Taubes equation](../../../../../../taubes-equation.md)

$$
\boxed{\Delta h+1-e^h=4\pi\sum_am_a\delta_{z_a},\qquad h\to0\text{ as }|z|\to\infty.}
$$

Near each zero, require $h=2m_a\log|z-z_a|+$ a smooth remainder. The planar existence theorem for this equation gives a solution for every finite multiset of prescribed points, unique in this decaying class; see [the original theorem](https://doi.org/10.1007/BF01197552). This elliptic existence result is the nontrivial analytic ingredient of the construction, not a linear superposition assumption.

Reconstruct $\Phi=e^{h/2+i\chi}$ and $A$ from the formulas above. The phase factors have integer winding, so $\Phi$ is single-valued. Near a zero, the modulus and phase combine into $(z-z_a)^{m_a}$ times a smooth nonvanishing factor. The singular part of $\nabla\chi$ cancels the rotated logarithmic-gradient part of $A$, so the physical fields extend smoothly through the cores. This produces the desired [Abelian Higgs vortices](../../../../../../nielsen-olesen-vortex.md) at the selected positions. Their [vortex number](../../../../../../vortex-number.md) is $N=\sum_am_a$. Replacing $(A,\Phi)$ by $(-A,\overline\Phi)$ constructs the negative-sign antivortex family; the positive construction does not assert arbitrary mixtures of positive and negative cores solve the same first-order equations.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
