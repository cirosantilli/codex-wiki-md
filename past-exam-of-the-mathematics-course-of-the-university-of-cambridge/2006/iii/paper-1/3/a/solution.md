<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [Lie group](../../../../../../lie-group.md) $G$ with identity $e$, its [Lie algebra](../../../../../../lie-algebra-split.md) as a set is the [tangent space](../../../../../../tangent-space.md) $T_eG$:

$$
\mathfrak g=\{\gamma'(0):\gamma:(-\varepsilon,\varepsilon)\to G\text{ smooth},\ \gamma(0)=e\}.
$$

The ambient embedding identifies these tangent vectors with vectors in $\mathbb R^N$. For a matrix [Lie group](../../../../../../lie-group.md), the identity is $I$ and the tangent vectors are matrices.

If $\gamma(t)\in\mathrm{SL}_n$ with $\gamma(0)=I$, put $A=\gamma'(0)$. The [determinant](../../../../../../determinant.md) expansion $\det(I+tA+o(t))=1+t\operatorname{tr}A+o(t)$ follows directly from its permutation formula: to first order only the diagonal entries contribute. Since $\det\gamma(t)=1$, differentiation gives $\operatorname{tr}A=0$. Thus

$$
\boxed{\operatorname{Lie}(\mathrm{SL}_n)\subseteq\mathfrak{sl}_n.}
$$

In fact equality holds: if $\operatorname{tr}A=0$, then $\exp(tA)$ has [determinant](../../../../../../determinant.md) $\exp(t\operatorname{tr}A)=1$ and derivative $A$ at zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
