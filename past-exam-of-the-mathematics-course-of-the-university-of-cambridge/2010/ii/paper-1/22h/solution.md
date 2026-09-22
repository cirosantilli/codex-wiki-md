<h1 id="22h/solution">Solution</h1>

↑ **Parent:** [22H](../22h.md)

The [Banach-Steinhaus theorem](../../../../../uniform-boundedness-principle.md), or [Uniform boundedness principle](../../../../../uniform-boundedness-principle.md), states that for a family $\mathcal T$ of [bounded linear operators](../../../../../continuous-linear-operator.md) from a [Banach space](../../../../../banach-space-split.md) $E$ to a normed space $F$, pointwise boundedness $\sup_{T\in\mathcal T}\|Tx\|<\infty$ for every $x\in E$ implies $\sup_T\|T\|<\infty$.

For its proof let $E_n=\{x:\sup_T\|Tx\|\leq n\}$. These are closed and their union is $E$. The [Baire category theorem](../../../../../baire-category-theorem.md) gives an $E_n$ with nonempty interior, containing a ball $B(x_0,r)$. For $\|h\|<r$, both $x_0$ and $x_0+h$ belong to $E_n$, so $\|Th\|\leq2n$ for every $T$. Scaling $h$ and taking a limit at the ball boundary gives $\|T\|\leq2n/r$, proving the theorem. The target need not be complete.

For the asserted bounded-set criterion, use the [Banach space](../../../../../banach-space-split.md) $X^*$, which is complete even if $X$ is not. Each $x\in S$ defines the bounded linear evaluation functional $J_x(f)=f(x)$ on $X^*$. The given hypothesis says this family is pointwise bounded. The [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) consequence in the question gives $\|J_x\|=\|x\|$, and uniform boundedness yields

$$
\boxed{\sup_{x\in S}\|x\|<\infty.}
$$

This proves that [weak boundedness implies norm boundedness](../../../../../weak-boundedness-implies-norm-boundedness.md); the two forms of boundedness coincide for a subset of a normed space.

Finally suppose the two continuous duals for $\|\cdot\|_1$ and $\|\cdot\|_2$ were equal as sets. The unit ball for norm two is bounded under every common continuous functional, using its norm-two continuity. Applying the preceding criterion in norm one bounds that ball in norm one; scaling gives $\|v\|_1\leq C\|v\|_2$. Reversing the roles gives $\|v\|_2\leq C'\|v\|_1$. The norms would be equivalent. Contrapositively, **inequivalent norms have different continuous duals**, supplying a linear functional continuous for one and discontinuous for the other.

## ↑ Ancestors (10)

1. [22H](../22h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
