<h1 id="a/2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The compact set $S(B_{c_0})$ is bounded, so $S$ is a [bounded linear operator](../../../../../continuous-linear-operator.md). For each $g\in Y^*$, the [continuous linear functional](../../../../../continuous-linear-functional.md) $g$ attains its maximum on that [compact set](../../../../../compact-space.md). Symmetry of $S(B_{c_0})$ implies that maximum is $\|S^*g\|$, so $S^*g$ attains its [norm](../../../../../norm.md) on $B_{c_0}$. By [norm attainment on the vanishing sequence space](../../../../../norm-attainment-on-the-vanishing-sequence-space.md),

$$
S^*(Y^*)\subseteq c_{00}\subset\ell_1.
$$

Regard the [Banach-space adjoint](../../../../../transpose-of-a-bounded-linear-operator.md) $S^*$ as a [bounded linear operator](../../../../../continuous-linear-operator.md) from the [Banach space](../../../../../banach-space-split.md) $Y^*$ into $c_{00}$ with its inherited $\ell_1$ [norm](../../../../../norm.md). The [completeness of the dual space](../../../../../completeness-of-the-dual-space.md) holds even if $Y$ is incomplete. The preceding [Baire category theorem](../../../../../baire-category-theorem.md) argument shows that $S^*$ has finite rank.

If $S^*(Y^*)=\operatorname{span}\{f_1,\ldots,f_r\}$, set $N=\bigcap_{j=1}^r\ker f_j$. For $x\in N$ and every $g\in Y^*$, $g(Sx)=(S^*g)(x)=0$. The [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) implies that [continuous linear functionals](../../../../../continuous-linear-functional.md) separate points of $Y$, so $Sx=0$. Thus $N\subseteq\ker S$, and

$$
\boxed{\operatorname{rank}S\leq\operatorname{codim}N\leq r<\infty.}
$$

This proves [compact closed-ball image forces finite rank on c0](../../../../../compact-closed-ball-image-forces-finite-rank-on-c0.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../split.md)
6. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
