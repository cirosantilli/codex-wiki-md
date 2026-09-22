<h1 id="s/1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the shifted normal proposal, $w(x)=e^{-\mu x+\mu^2/2}$ and the estimator is

$$
\hat p_N=\frac1N\sum_i1_{\{X_i>z\}}e^{-\mu X_i+\mu^2/2},
\qquad X_i\sim N(\mu,1).
$$

Let $\bar\Phi=1-\Phi$. Completing the square gives its unaveraged second moment

$$
I(\mu)=\int_z^\infty\frac{p(x)^2}{q_\mu(x)}\,dx
=e^{\mu^2}\bar\Phi(z+\mu).
$$

The variance is $[I(\mu)-\bar\Phi(z)^2]/N$, so only $I$ needs minimization. It tends to infinity at both ends of the real $\mu$ axis and has a finite minimizer. Differentiation at a minimizer yields

$$
2\mu\,\bar\Phi(z+\mu)=\varphi(z+\mu).
$$

For a standard normal variable, integration of $x\varphi(x)=-\varphi'(x)$ shows $E_p[X\mid X>a]=\varphi(a)/\bar\Phi(a)$. Consequently

$$
\boxed{2\mu=E_p[X\mid X>z+\mu].}
$$

The shift is chosen to reduce the second moment of the weighted rare-event indicator, rather than merely to increase the proposal's tail probability.

## ↑ Ancestors (13)

1. [D](../d.md)
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
