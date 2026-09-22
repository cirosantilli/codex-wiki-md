<h1 id="11/c/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

For real orthonormal column [vectors](../../../../../vector.md), $u^Tu=v^Tv=1$ and $u^Tv=v^Tu=0$. Expand using associativity of [matrix multiplication](../../../../../matrix-multiplication.md):

$$
\begin{aligned}
(uu^T+vv^T)^2
&=u(u^Tu)u^T+u(u^Tv)v^T+v(v^Tu)u^T+v(v^Tv)v^T\\
&=uu^T+vv^T.
\end{aligned}
$$

Hence

$$
\boxed{M=uu^T+vv^T\text{ is idempotent}.}
$$

More precisely, it is the [orthogonal projection](../../../../../orthogonal-projection.md) onto the span of $u,v$: it fixes both [vectors](../../../../../vector.md) and annihilates every [vector](../../../../../vector.md) orthogonal to both.

The transpose convention presumes real [vectors](../../../../../vector.md), or the explicitly stated bilinear identities above. For complex [vectors](../../../../../vector.md) orthonormal in the [Hermitian inner product](../../../../../hermitian-inner-product.md), the correct [orthogonal projection](../../../../../orthogonal-projection.md) is $uu^\dagger+vv^\dagger$. The printed transpose formula need not work in that setting: $u=(i,0)^T$ and $v=(0,1)^T$ are Hermitian-orthonormal, but $uu^T+vv^T=\operatorname{diag}(-1,1)$ has square $I_2$, which is different from itself.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [C](../../c.md)
3. [11](../../../11.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the mathematical methods I course of the University of Oxford](../../../../split.md)
6. [Mathematical methods I course of the University of Oxford](../../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
