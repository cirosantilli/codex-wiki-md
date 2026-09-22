<h1 id="1/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose the [continuously differentiable functions](../../../../../continuously-differentiable-function.md)

$$
f_n(x)=\sqrt{x^2+n^{-2}}.
$$

The estimate $\sqrt{a^2+b^2}\leq a+b$ for $a,b\geq0$ gives

$$
0\leq f_n(x)-|x|\leq\frac1n,\qquad
\|f_n-|\cdot|\|_\infty=\frac1n.
$$

Thus $f_n\to|\cdot|$ by [uniform convergence](../../../../../uniform-convergence.md), and the [triangle inequality](../../../../../triangle-inequality.md) gives $\|f_n-f_m\|_\infty\leq n^{-1}+m^{-1}$. The [sequence](../../../../../sequence.md) is a [Cauchy sequence](../../../../../cauchy-sequence.md) in $X$, but its unique possible [supremum norm](../../../../../supremum-norm.md) limit is $x\mapsto|x|$, which is not [differentiable](../../../../../differentiable-function.md) at zero. That limit is outside $X$, so

$$
\boxed{(C^1([-1,1]),\|\cdot\|_\infty)\text{ is incomplete}.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
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
