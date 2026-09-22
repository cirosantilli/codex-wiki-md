<h1 id="a/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\rho=r-\sqrt{r^2-1}$. Since $r>1$, $0<\rho<1$ and $\rho^2-2r\rho+1=0$. The nonzero square-summable sequence $\beta_j=\rho^{j-1}$ defines a [continuous linear functional](../../../../../continuous-linear-functional.md) on $\ell_2$ by

$$
f(\alpha)=\sum_{j\geq1}\alpha_j\rho^{j-1}.
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) proves [continuity](../../../../../continuous-function.md). For every $k$,

$$
f(x_k)=\rho^{k-1}(1-2r\rho+\rho^2)=0.
$$

Hence $f$ vanishes on the [closed linear span](../../../../../closed-linear-span.md) $M$, but $f(e_1)=1$. Therefore

$$
\boxed{M\ne\ell_2.}
$$

More precisely, any vector in the [orthogonal complement](../../../../../orthogonal-complement.md) of $M$ satisfies the recurrence $\beta_{k+2}-2r\beta_{k+1}+\beta_k=0$. Its roots are $r\pm\sqrt{r^2-1}$, one less than one and the other greater than one. Square summability eliminates the growing solution, so $M^\perp$ is exactly the span of $(\rho^{j-1})$. Thus $M=\ker f$ is a closed hyperplane of codimension one. This is [annihilator of a second-difference span in l2](../../../../../annihilator-of-a-second-difference-span-in-l2.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
