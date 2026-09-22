<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**Zero is a strict weak local minimizer, but is not a strong local minimizer.** The [derivative](../../../../../derivative.md) integrand has expansion $\cosh v\cos(v^2)=1+v^2/2+O(v^4)$, so for small $|v|$ it is at least $1+3v^2/8$. [Concavity](../../../../../concave-function.md) gives $(1+u^2)^{1/4}\leq1+u^2/4$ for every real $u$. Therefore, when $\|u'\|_\infty$ is small,

$$
I(u)-I(0)\geq\frac38\int_0^1u'^2-\frac12\int_0^1u^2\geq\frac18\int_0^1u'^2,
$$

using $\int u^2\leq\tfrac12\int u'^2$. This proves strict weak minimality.

For the strong claim, let $v_N(x)=\sqrt\pi\,\operatorname{dist}(x,N^{-1}\mathbb Z)$. Its amplitude tends to zero and its [derivative](../../../../../derivative.md) is $\pm\sqrt\pi$ [almost everywhere](../../../../../almost-everywhere.md), so the [derivative](../../../../../derivative.md) integrand is the constant $-\cosh\sqrt\pi$. The other integrand term is at most $-2$. Hence

$$
\boxed{I(v_N)\leq-\cosh\sqrt\pi-2<-1=I(0),\qquad\|v_N\|_\infty\to0.}
$$

This disproves strong minimality. The same obstruction is detected by the [Weierstrass necessary condition](../../../../../weierstrass-necessary-condition.md), since the supporting-tangent inequality at slope zero fails at $v=\sqrt\pi$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the calculus of variations course of the University of Oxford](../../../../split.md)
6. [Calculus of variations course of the University of Oxford](../../../../../calculus-of-variations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
