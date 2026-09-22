<h1 id="7b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The differential [Gauss law](../../../../../../gauss-s-law.md) is $\nabla\cdot\mathbf E=\rho/\epsilon_0$. On a large ball $B_R$, the product rule and $\nabla\phi=-\mathbf E$ give

$$
\rho\phi=\epsilon_0\nabla\cdot(\phi\mathbf E)+\epsilon_0|\mathbf E|^2.
$$

The [divergence theorem](../../../../../../divergence-theorem.md) consequently expresses the [electrostatic energy](../../../../../../electrostatic-energy.md) as

$$
\frac12\int_{B_R}\rho\phi\,dV=\frac{\epsilon_0}{2}\int_{B_R}|\mathbf E|^2\,dV+\frac{\epsilon_0}{2}\int_{\partial B_R}\phi\mathbf E\cdot\mathbf n\,dS.
$$

For a localized charge distribution with the [electric potential](../../../../../../electric-potential.md) chosen to vanish at infinity, $\phi=O(R^{-1})$ and $\mathbf E=O(R^{-2})$, so the surface term is $O(R^{-1})$ and tends to zero. More generally, it suffices to assume that this boundary integral vanishes. Passing to all space gives

$$
\boxed{U=\frac{\epsilon_0}{2}\int_{\mathbb R^3}|\mathbf E|^2\,dV.}
$$

The physical decay and potential reference are relevant: $\mathbf E\to0$ by itself does not specify the additive constant in $\phi$. Adding a constant $C$ changes the charge-based expression by $CQ/2$ when the total charge is $Q$, while leaving the field unchanged. The zero-at-infinity potential is the usual reference implicit in this all-space [electrostatic energy](../../../../../../electrostatic-energy.md) formula.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [7B](../../7b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
