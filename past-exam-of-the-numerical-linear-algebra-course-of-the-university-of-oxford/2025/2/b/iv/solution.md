<h1 id="2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Because $r<n$, choose a [unit vector](../../../../../unit-vector.md) $v$ in the [null space](../../../../../kernel-of-a-linear-map-split.md) of $X^T$, so that $v^TX=0$. Let $J\in\mathbb R^{m\times n}$ have [orthonormal](../../../../../orthonormal-set.md) columns, for example the first $n$ columns of $I_m$, and choose a real number $\alpha>1$. Set

$$
\boxed{A=J\bigl(I_n+(\alpha-1)vv^T\bigr)}.
$$

Its [singular value](../../../../../singular-value.md) along $v$ is $\alpha$, and its other [singular values](../../../../../singular-value.md) are $1$. Thus $\sigma_1(A)=\alpha>1=\sigma_2(A)$. Meanwhile $AX=JX$. If $X$ has [full column rank](../../../../../full-column-rank.md), the [column space](../../../../../column-space.md) of the thin [QR decomposition](../../../../../qr-decomposition.md) is exactly $\operatorname{range}(JX)$, which is [orthogonal](../../../../../orthogonal-vectors.md) to $Jv$. Hence $PJv=0$ for $P=QQ^T$, and

$$
\|(I_m-P)A\|_2\geq\|(I_m-P)Av\|_2=\|\alpha Jv\|_2=\alpha.
$$

Conversely, an [orthogonal projection](../../../../../orthogonal-projection.md) is a contraction in the [Euclidean norm](../../../../../euclidean-norm.md), so $\|(I_m-P)A\|_2\leq\|A\|_2=\alpha$. Therefore

$$
\boxed{\|A-\widehat A\|_2=\sigma_1(A)=\alpha>\sigma_2(A)=1}.
$$

If $X$ is rank deficient, complete the [QR decomposition](../../../../../qr-decomposition.md) within $J(v^\perp)$: this space has dimension $n-1\geq r$ and contains all columns of $JX$, so the required [orthonormal](../../../../../orthonormal-set.md) completion exists there. The same proof applies. For rank-deficient data the choice of unused columns of $Q$ matters; the construction specifies a valid choice. If $Q$ instead contains only a [basis](../../../../../basis.md) of $\operatorname{range}(AX)$, the conclusion holds without any completion. A fixed sampling [matrix](../../../../../matrix.md) can thus miss the unique largest [singular value](../../../../../singular-value.md) completely.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the numerical linear algebra course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra course of the University of Oxford](../../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
