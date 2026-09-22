<h1 id="b/4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [descent lemma](../../../../../descent-lemma.md) follows by integrating the [gradient](../../../../../gradient.md) along the line and using its [Lipschitz continuity](../../../../../lipschitz-continuity.md):

$$
f(x+\alpha p)\leq f(x)+\alpha g(x)^Tp+\frac\gamma2\alpha^2\|p\|_2^2,\qquad\alpha\geq0.
$$

This upper bound is at most the right side of the [Armijo condition](../../../../../armijo-condition.md) when $\alpha[(1-\beta)g^Tp+\gamma\alpha\|p\|_2^2/2]\leq0$. Since $g^Tp<0$, it holds for

$$
\boxed{0\leq\alpha\leq\alpha_{\max}=\frac{2(1-\beta)(-g^Tp)}{\gamma\|p\|_2^2}=\frac{2(\beta-1)g^Tp}{\gamma\|p\|_2^2}.}
$$

The zero step gives equality; every positive step in this interval satisfies the prescribed sufficient-decrease test.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
