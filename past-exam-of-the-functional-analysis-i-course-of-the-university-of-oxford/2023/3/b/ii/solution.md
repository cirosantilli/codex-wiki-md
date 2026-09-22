<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $\psi=\psi_{x_0}$; its value at $x_0$, if that point is in $(0,1)$, may be assigned arbitrarily because [Lp spaces](../../../../../lp-space.md) identify [functions](../../../../../function-split.md) equal [almost everywhere](../../../../../almost-everywhere.md). Its [L-infinity norm](../../../../../l-infinity-norm.md) is one.

The supplied estimate shows that $\psi$ cannot agree [almost everywhere](../../../../../almost-everywhere.md) with any [continuous function](../../../../../continuous-function.md) $q$: choosing $g=-q$ would give $0\geq|q(x_0)|+1$. Hence

$$
V=C([0,1])\oplus\langle\psi\rangle
$$

is a [direct sum](../../../../../direct-sum.md), so every element has a unique expression $g+c\psi$.

For any complex $a$ with $|a|\leq1$, define the [linear functional](../../../../../linear-functional.md)

$$
L_a(g+c\psi)=g(x_0)+ca.
$$

If $c\ne0$, the supplied estimate, applied to $g/c$, and [absolute homogeneity of a norm](../../../../../absolute-homogeneity-of-a-norm.md) give

$$
\|g+c\psi\|_\infty=|c|\|g/c+\psi\|_\infty
\geq|g(x_0)|+|c|
\geq|g(x_0)+ca|.
$$

For $c=0$, the same bound follows from [point evaluation](../../../../../point-evaluation-functional.md). Thus $\|L_a\|\leq1$, and $L_a(1)=1$ makes its [operator norm](../../../../../operator-norm.md) exactly one. The [complex Hahn-Banach theorem](../../../../../complex-hahn-banach-theorem.md) extends $L_a$ to a norm-one [linear functional](../../../../../linear-functional.md) on all of $X$, with value $a$ at $\psi$.

Conversely every norm-one extension satisfies $|\ell_{x_0}(\psi)|\leq\|\psi\|_\infty=1$. We have therefore determined all possible values:

$$
\boxed{\{\ell_{x_0}(\psi_{x_0}):\ell_{x_0}\text{ is a norm-one extension of }E_{x_0}\}
=\{a\in\mathbb C:|a|\leq1\}.}
$$

In particular, taking $a=0$ and $a=1$ proves [nonuniqueness of norm-preserving point evaluation extensions](../../../../../nonuniqueness-of-norm-preserving-point-evaluation-extensions.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis I course of the University of Oxford](../../../../split.md)
6. [Functional analysis I course of the University of Oxford](../../../../../functional-analysis-i-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
