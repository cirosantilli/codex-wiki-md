<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [integration by parts](../../../../../integration-by-parts.md) with a [complex conjugate](../../../../../complex-conjugate.md), so that the argument also covers complex-valued [eigenfunctions](../../../../../eigenfunction.md). The coefficient functions are understood to be real. For a nonzero [eigenfunction](../../../../../eigenfunction.md) $u$ with [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md),

$$
\begin{aligned}
\lambda\int_\alpha^\beta |u|^2\,dx
&=\int_\alpha^\beta\overline u\,Mu\,dx\\
&=\bigl[a\overline u\,u'\bigr]_\alpha^\beta-\int_\alpha^\beta a|u'|^2\,dx+\int_\alpha^\beta b|u|^2\,dx\\
&=-\int_\alpha^\beta a|u'|^2\,dx+\int_\alpha^\beta b|u|^2\,dx.
\end{aligned}
$$

The denominator is strictly positive and the numerator is real. Consequently the [eigenvalue](../../../../../eigenvalue.md) satisfies

$$
\boxed{\lambda=\frac{\int_\alpha^\beta(b|u|^2-a|u'|^2)\,dx}{\int_\alpha^\beta|u|^2\,dx}\in\mathbb R.}
$$

This is the [Rayleigh quotient](../../../../../rayleigh-quotient.md) for the sign convention used here. Positivity of $a$ is unnecessary for this particular reality argument; real coefficients and disappearance of the endpoint term are what matter.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
