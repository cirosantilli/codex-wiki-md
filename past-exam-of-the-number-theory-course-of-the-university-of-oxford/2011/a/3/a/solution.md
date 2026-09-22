<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Fundamental theorem of symmetric polynomials](../../../../../fundamental-theorem-of-symmetric-polynomials.md) states that every symmetric [polynomial](../../../../../polynomial-split.md) in $n$ variables over a [field](../../../../../field.md) is a [polynomial](../../../../../polynomial-split.md) in the elementary symmetric polynomials, uniquely so. For the three roots, [Vieta's formulas](../../../../../vieta-s-formulas.md) give $e_1=0$, $e_2=p$, $e_3=-q$.

The squared product of root differences is symmetric. Expansion in elementary symmetric polynomials gives

$$
\begin{aligned}
(\alpha-\beta)^2(\beta-\gamma)^2(\gamma-\alpha)^2
&=e_1^2e_2^2-4e_2^3-4e_1^3e_3-27e_3^2+18e_1e_2e_3\\
&=\boxed{-4p^3-27q^2.}
\end{aligned}
$$

One can verify the displayed identity simply by substituting the definitions of $e_1,e_2,e_3$ and expanding; it is the cubic [polynomial discriminant](../../../../../polynomial-discriminant.md).

If the cubic is irreducible, its roots are distinct in characteristic zero, so $\delta\ne0$. Its [Galois group](../../../../../galois-group.md) is a transitive [subgroup](../../../../../subgroup.md) of $S_3$, hence either $A_3$ or $S_3$. A permutation of the roots multiplies $\delta$ by its sign. The fixed-[field](../../../../../field.md) assertion of the [Fundamental theorem of Galois theory](../../../../../fundamental-theorem-of-galois-theory.md) therefore gives $\delta\in\mathbb Q$ exactly when all [group](../../../../../group-split.md) elements are even. Thus

$$
\boxed{\operatorname{Gal}(f)=A_3\ \text{if }\delta\in\mathbb Q,\qquad
\operatorname{Gal}(f)=S_3\ \text{otherwise}.}
$$

For example, $f=x^3-3x-1$ has no rational root: neither $1$ nor $-1$ is a root, and these are the only possibilities by the [rational root theorem](../../../../../rational-root-theorem.md). Its [discriminant](../../../../../discriminant.md) is $108-27=81$, so $\delta=\pm9\in\mathbb Q$ and its [group](../../../../../group-split.md) is $A_3$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the number theory course of the University of Oxford](../../../../split.md)
6. [Number theory course of the University of Oxford](../../../../../number-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
