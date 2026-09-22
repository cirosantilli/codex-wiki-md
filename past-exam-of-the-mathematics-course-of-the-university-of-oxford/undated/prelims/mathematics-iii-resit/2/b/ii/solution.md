<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The inverse [change of variables](../../../../../../../change-of-variables-formula.md) is $x=v/(1+u)$, $y=uv/(1+u)$. Thus the triangular region becomes

$$
0\le u\le1,\qquad 0\le v\le1+u.
$$

The upper limit depends on $u$: the new region is not a [rectangle](../../../../../../../rectangle.md). The absolute inverse [Jacobian determinant](../../../../../../../jacobian-determinant.md) is $x^2/(x+y)$, so the [change of variables formula](../../../../../../../change-of-variables-formula.md) cancels the rational factor in the [integrand](../../../../../../../integrand.md):

$$
\begin{aligned}
I&=\int_0^1\int_0^{1+u}e^v\,dv\,du
=\int_0^1(e^{1+u}-1)\,du\\
&=\boxed{e^2-e-1.}
\end{aligned}
$$

Although the original [integrand](../../../../../../../integrand.md) is undefined at the vertex $x=y=0$, its nonnegative [improper integral](../../../../../../../improper-integral.md) exists. One can apply the [change of variables formula](../../../../../../../change-of-variables-formula.md) on $x\ge\varepsilon$ and let $\varepsilon\downarrow0$ by the [monotone convergence theorem](../../../../../../../monotone-convergence-theorem.md); the transformed [integrand](../../../../../../../integrand.md) has the finite [integral](../../../../../../../integral-split.md) just computed.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Mathematics III resit](../../../../mathematics-iii-resit-split.md)
5. [Prelims](../../../../split.md)
6. [Undated](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
