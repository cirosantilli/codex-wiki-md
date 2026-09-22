<h1 id="3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Replacing a minimizer by its absolute value does not increase its gradient norm, so choose a nonnegative minimizer $P$. The [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) is

$$
-\Delta P+P+\frac\eta4|x|^2P=\mu P^3
$$

for a [Lagrange multiplier](../../../../../../lagrange-multiplier.md) $\mu$. Multiplication by $P$ and integration show that

$$
\mu M=\int|\nabla P|^2+\int|P|^2+\frac\eta4\int|x|^2|P|^2>0,
$$

so $\mu>0$. Set $P_\eta=\sqrt\mu P$. Then $P_\eta$ is nonzero, belongs to $H^1(\mathbb R^2)$, and satisfies the [trapped focusing cubic ground-state equation](../../../../../../trapped-focusing-cubic-ground-state-equation.md)

$$
\boxed{\Delta P_\eta-P_\eta-\frac\eta4|x|^2P_\eta+P_\eta^3=0}.
$$

Standard elliptic regularity and the [strong minimum principle for elliptic operators](../../../../../../strong-minimum-principle-for-elliptic-operators.md) make the nonnegative solution positive.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [3](../../3.md)
3. [Paper 154](../../../paper-154-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
