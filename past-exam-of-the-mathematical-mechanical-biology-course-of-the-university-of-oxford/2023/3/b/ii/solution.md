<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $W_i=\partial W/\partial\alpha_i$, evaluated at $(\alpha^{-1/2},\alpha^{-1/2},\alpha)$. Applying the [chain rule](../../../../../chain-rule.md) to the reduced [strain energy density](../../../../../strain-energy-density.md) gives

$$
\hat W'(\alpha)
=-\frac12\alpha^{-3/2}W_1-\frac12\alpha^{-3/2}W_2+W_3.
$$

Multiply by $\alpha$ and use $\alpha_1=\alpha_2=\alpha^{-1/2}$:

$$
\alpha\hat W'(\alpha)
=\alpha_3W_3-\frac12\alpha_1W_1-\frac12\alpha_2W_2.
$$

The transverse symmetry specified in the hint has $W_1=W_2$. Thus

$$
\boxed{\alpha\hat W'(\alpha)=\alpha_3W_3-\alpha_1W_1.}
$$

The lateral faces have zero [traction](../../../../../traction.md), so their diagonal [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md) components satisfy $t_1=t_2=0$. The [hydrostatic pressure](../../../../../hydrostatic-pressure.md) enforcing [elastic incompressibility](../../../../../elastic-incompressibility.md) is therefore $p=\alpha_1W_1=\alpha_2W_2$, and the axial component simplifies to

$$
\boxed{t_3=\alpha_3W_3-p=\alpha\hat W'(\alpha).}
$$

This elimination of the [Lagrange multiplier](../../../../../lagrange-multiplier.md) $p$ is what makes the reduced [strain energy density](../../../../../strain-energy-density.md) useful for the spring balance.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the mathematical mechanical biology course of the University of Oxford](../../../../split.md)
6. [Mathematical mechanical biology course of the University of Oxford](../../../../../mathematical-mechanical-biology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
