<h1 id="b/7/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [Lipschitz gradient](../../../../../lipschitz-gradient.md) with constant $\gamma>0$ gives the [descent lemma](../../../../../descent-lemma.md)

$$
f(x+\alpha p)\leq f(x)+\alpha g^Tp+\frac\gamma2\alpha^2\|p\|_2^2.
$$

For $\alpha>0$, this upper bound is at most $f(x)+\alpha\beta g^Tp$ whenever $\tfrac\gamma2\alpha\|p\|_2^2\leq(\beta-1)g^Tp$. Since $p$ is a [descent direction](../../../../../descent-direction.md), the right side is positive. Thus the [Armijo condition](../../../../../armijo-condition.md) holds throughout

$$
\boxed{0\leq\alpha\leq\alpha_{\max}=\frac{2(\beta-1)g^Tp}{\gamma\|p\|_2^2}.}
$$

At $\alpha=0$ it holds by equality. If the gradient Lipschitz constant can be taken as zero, the objective is affine and every positive step along a descent direction passes this sufficient-decrease test.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
