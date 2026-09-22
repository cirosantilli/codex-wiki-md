<h1 id="s/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the necessary [support condition for importance sampling](../../../../../support-condition-for-importance-sampling.md), $p\ll q$; the source's density assumptions alone do not ensure it. Put $\mu=E_p f$ and $w=p/q=(Z_q/Z_p)\tilde p/\tilde q$. The [importance sampling](../../../../../importance-sampling.md) estimator is

$$
\boxed{\hat\mu_N=\frac1N\sum_{i=1}^Nw(X_i)f(X_i).}
$$

Integration under $q$ gives $E_q[wf]=\int pf=\mu$, proving unbiasedness. Independence gives

$$
\boxed{\operatorname{Var}(\hat\mu_N)=\frac1N
\left(\int\frac{p(x)^2f(x)^2}{q(x)}\,dx-\mu^2\right).}
$$

This variance is finite precisely when the first integral is finite. The assumption $E_pf^2<\infty$ ensures target square integrability, but need not ensure square integrability after importance reweighting; the variance can be infinite.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [S](../../../s.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
