<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

There is no need to assume that the original zeroth-order coefficient is nonpositive. Set $c_+=\max(c,0)$ and $\widetilde c=\min(c,0)$, and use the [uniformly elliptic operator](../../../../../../uniformly-elliptic-operator.md)

$$
\widetilde L=a^{ij}D_{ij}+b^iD_i+\widetilde c.
$$

Because $u\geq0$ and $f\leq0$,

$$
\widetilde Lu=f-c_+u\leq0.
$$

Now $\widetilde c\leq0$, so the [strong minimum principle for elliptic operators](../../../../../../strong-minimum-principle-for-elliptic-operators.md) applies. If $u$ vanished at an interior point of the [connected](../../../../../../connected-space.md) domain, this principle would force $u$ to vanish identically. The given nontriviality therefore proves

$$
\boxed{u(x)>0\qquad(x\in\Omega).}
$$

**Every nontrivial nonnegative solution is strictly positive inside.** This uses the nondivergence-form [strong minimum principle for elliptic operators](../../../../../../strong-minimum-principle-for-elliptic-operators.md); the divergence-form [Harnack inequality for uniformly elliptic divergence-form equations](../../../../../../harnack-inequality-for-uniformly-elliptic-divergence-form-equations.md) in part (a) is not being applied to this operator.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
