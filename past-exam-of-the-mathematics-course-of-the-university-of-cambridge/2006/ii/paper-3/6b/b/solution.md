<h1 id="6b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $rN>a$ and $p>0$, a nonzero infected [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) requires $S_*=a/r$. Using $aI_*=pR_*$ and population conservation gives

$$
\boxed{S_*=\frac ar,\qquad I_*=\frac{p}{a+p}\left(N-\frac ar\right),\qquad R_* =\frac{a}{a+p}\left(N-\frac ar\right).}
$$

Eliminate $R=N-S-I$ before assessing [stability](../../../../../../stability-of-a-numerical-method.md), since perturbations must preserve the total population. The resulting [Jacobian matrix](../../../../../../jacobian-matrix.md) at this [endemic equilibrium](../../../../../../endemic-equilibrium.md) is

$$
J=\begin{pmatrix}-p-rI_*&-p-a\\rI_*&0\end{pmatrix},\quad \operatorname{tr}J=-\frac{p(p+rN)}{a+p},\quad\det J=p(rN-a).
$$

Its [trace](../../../../../../matrix-trace.md) is negative and its [determinant](../../../../../../determinant.md) positive, so both [eigenvalues](../../../../../../eigenvalue.md) have negative real part: **the endemic equilibrium is locally asymptotically stable on the fixed-population plane**. The full three-variable system has a neutral direction corresponding to changing the conserved population.

Writing $\kappa=rN-a>0$, as $p\to0$ the [trace](../../../../../../matrix-trace.md) is $-prN/a+O(p^2)$ and the [determinant](../../../../../../determinant.md) is $p\kappa$. Hence the [discriminant](../../../../../../discriminant.md) $(\operatorname{tr}J)^2-4\det J=-4p\kappa+O(p^2)<0$. As $p\to\infty$, the [trace](../../../../../../matrix-trace.md) is $-p-\kappa+O(p^{-1})$ and the [determinant](../../../../../../determinant.md) is again $p\kappa$, giving a positive [discriminant](../../../../../../discriminant.md) $p^2+O(p)$. Both quantities are $O(p)$ in both limits, but the [eigenvalues](../../../../../../eigenvalue.md) are **complex for sufficiently small $p$ and real for sufficiently large $p$**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6B](../../6b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
