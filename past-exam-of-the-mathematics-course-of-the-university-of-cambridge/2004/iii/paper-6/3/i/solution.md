<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $x,y\in B$, write $L_x(y)=xy$ and $R_y(x)=xy$. Separate [continuity](../../../../../../continuous-function.md) and [linearity](../../../../../../linearity.md) make both maps [bounded linear operators](../../../../../../continuous-linear-operator.md). For each fixed $y$,

$$
\sup_{\|x\|\leq1}\|L_x y\|=\sup_{\|x\|\leq1}\|R_yx\|\leq\|R_y\|<\infty.
$$

The [Uniform boundedness principle](../../../../../../uniform-boundedness-principle.md) therefore gives $C<\infty$ such that $\|L_x\|\leq C$ whenever $\|x\|\leq1$. Scaling yields

$$
\|xy\|\leq C\|x\|\|y\|.
$$

For completeness, the relevant [Uniform boundedness principle](../../../../../../uniform-boundedness-principle.md) follows from the [Baire category theorem](../../../../../../baire-category-theorem.md) as follows. For a pointwise bounded family $\mathcal T$ of [bounded linear operators](../../../../../../continuous-linear-operator.md) on a [Banach space](../../../../../../banach-space-split.md), the [closed sets](../../../../../../closed-set.md) $E_m=\{y:\sup_{T\in\mathcal T}\|Ty\|\leq m\}$ cover the space. One $E_m$ contains an [open ball](../../../../../../open-ball.md) $B(y_0,r)$. Subtracting the bounds for $y_0$ and $y_0+h$, with $\|h\|<r$, gives $\sup_T\|Th\|\leq2m$. Applying this to $h=(r/2)u$, $\|u\|\leq1$, bounds every [operator norm](../../../../../../operator-norm.md) by $4m/r$.

Define the new [norm](../../../../../../norm.md) by

$$
\boxed{\|x\|_* =\|L_x\|.}
$$

It is a [norm](../../../../../../norm.md) because $L_xe=x$, so $L_x=0$ implies $x=0$. The [triangle inequality](../../../../../../triangle-inequality.md) and scalar homogeneity follow from those of the [operator norm](../../../../../../operator-norm.md). Moreover,

$$
\frac{\|x\|}{\|e\|}\leq\|L_x\|\leq C\|x\|,
$$

so it is equivalent to the original [norm](../../../../../../norm.md) and remains complete. By [associativity](../../../../../../associative-property.md), $L_{xy}=L_xL_y$, and the [submultiplicativity](../../../../../../submultiplicativity.md) of the [operator norm](../../../../../../operator-norm.md) proves

$$
\boxed{\|xy\|_*\leq\|x\|_*\|y\|_*.}
$$

This is [renorming a separately continuous Banach algebra](../../../../../../renorming-a-separately-continuous-banach-algebra.md). It even gives $\|e\|_*=1$. If the algebra is the zero space, the conclusion is immediate separately.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
