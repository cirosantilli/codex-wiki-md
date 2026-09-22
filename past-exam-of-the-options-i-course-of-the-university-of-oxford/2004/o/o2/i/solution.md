<h1 id="o/o2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For nondegenerate design let $S_{xx}=\sum_i x_i^2>0$. Maximizing the Gaussian likelihood over the mean parameters is equivalent to minimizing $\sum_i(Y_i-\alpha-\beta x_i)^2$. Since $\sum_ix_i=0$, the [normal equations](../../../../../normal-equation.md) separate:

$$
\boxed{\widehat\alpha=\bar Y,\qquad\widehat\beta=\frac{\sum_ix_iY_i}{S_{xx}}.}
$$

Its error is the [linear combination](../../../../../linear-combination.md) $\widehat\beta-\beta=\sum_ix_i\epsilon_i/S_{xx}$. Independence and normality therefore give

$$
\boxed{\widehat\beta\sim N(\beta,\sigma^2/S_{xx}).}
$$

If every design point is zero, the slope is not identifiable and no such slope estimator can be inferred; the standard regression answer assumes the stated nondegeneracy.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [O2](../../o2.md)
3. [O](../../../o.md)
4. [2004](../../../../2004-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
