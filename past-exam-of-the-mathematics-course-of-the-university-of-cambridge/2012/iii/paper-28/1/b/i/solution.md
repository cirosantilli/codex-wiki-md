<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\mathcal O=\{x:|x|\leq1\}$. First, $\mathcal O$ is compact. A compact neighborhood of zero contains a sufficiently small closed ball $t^m\mathcal O$, since $|t|^m\to0$; that ball is closed in the compact neighborhood. Scaling back proves compactness of $\mathcal O$. Also $K$ is complete: a [Cauchy sequence](../../../../../../../cauchy-sequence.md) has a tail in a translate of a compact neighborhood, hence a convergent subsequence, and the Cauchy condition makes the whole sequence converge. This is the [completeness of locally compact nontrivially valued fields](../../../../../../../completeness-of-locally-compact-nontrivially-valued-fields.md) argument.

The additive subgroup $t\mathcal O$ is open: a sufficiently small ball around any of its points stays in $t\mathcal O$ by the ultrametric inequality. Thus the compact discrete quotient $\mathcal O/t\mathcal O$ is finite. Choose a set $A\subset\mathcal O$ of representatives, with zero representing the zero coset. For $x\in\mathcal O$, recursively choose $a_n\in A$ and $x_{n+1}\in\mathcal O$ such that $x_n=a_n+t x_{n+1}$, beginning with $x_0=x$. Then

$$
x=\sum_{j=0}^{m-1}a_jt^j+t^m x_m,\qquad |t^m x_m|\leq|t|^m\longrightarrow0.
$$

For arbitrary $x\in K$, multiply first by a large power of $t$ to put it in $\mathcal O$, then divide the resulting expansion by that power. This gives the [digit expansion with a nonuniformizer](../../../../../../../digit-expansion-with-a-nonuniformizer.md).

For uniqueness, take the first exponent $r$ at which two expansions differ. After dividing their difference by $t^r$, all the later terms belong to the closed subgroup $t\mathcal O$, whereas $a_r-b_r$ does not, because the representatives are distinct. The difference cannot be zero. Conversely every series with coefficients in $A$ and only finitely many nonzero negative-index terms converges by completeness and $|t|<1$. **Every element therefore has a unique expansion $\boxed{x=\sum_{n\geq r}a_n t^n}$**, with the harmless initial zero coefficients understood as part of the same indexed series. No assumption that $t$ is a [uniformizer](../../../../../../../uniformizer.md) is needed.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 28](../../../../paper-28-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
