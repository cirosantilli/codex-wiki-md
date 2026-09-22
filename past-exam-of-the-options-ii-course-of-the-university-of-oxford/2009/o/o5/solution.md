<h1 id="o/o5/solution">Solution</h1>

↑ **Parent:** [O5](../o5.md)

For unrestricted category probabilities, the [log-likelihood](../../../../log-likelihood.md) is $\sum_i n_i\log\pi_i$ subject to $\sum_i\pi_i=1$. A multiplier gives $n_i/\pi_i$ constant, hence the unique maximum, because all counts are positive and the [log-likelihood](../../../../log-likelihood.md) is strictly concave:

$$
\boxed{\widehat\pi_i=n_i/n}.
$$

The [likelihood ratio test](../../../../likelihood-ratio-test.md) compares this saturated maximum with the maximum under the parametric model. Twice the log ratio is

$$
2\sum_i n_i\log\frac{n_i/n}{\pi_i(\widehat\theta)}=\Lambda(\widehat\theta).
$$

For $k$ bins and one regular fitted parameter, its usual large-sample reference distribution is $\chi^2_{k-2}$; reject for a sufficiently large value. Under a fully specified parameter $\theta_0$, use $\Lambda(\theta_0)$ and $\chi^2_{k-1}$. This relies on an identifiable interior fit and adequate expected bin counts.

For individual ungrouped abundances, let $S$ be the number of species and $T$ the total number of individuals. The logarithmic-series model gives

$$
\ell(\theta)=-S\log[-\log(1-\theta)]+T\log\theta+C,\qquad0<\theta<1.
$$

Its score vanishes when

$$
\boxed{\frac{-\widehat\theta}{(1-\widehat\theta)\log(1-\widehat\theta)}=\frac TS}.
$$

The left side increases continuously from one to infinity. One way to see strict increase is to set $t=-\log(1-\theta)>0$, making it $(e^t-1)/t$, whose derivative is positive because $e^t(t-1)+1$ increases from zero. The score has the sign of $T/S$ minus this increasing [function](../../../../function-split.md), so this is the unique maximum. Bisection on $(0,1)$ is a robust numerical method; Newton's method is another option.

There are two fits implicit in the supplied presentation. Using the ungrouped sufficient statistics gives $\widehat\theta_{\rm full}\approx0.944228$. By contrast the displayed ten-bin deviance is minimized near **$0.93$**, so that is the table-based estimate $\widehat\theta_{\rm grouped}$. Grouping the upper tail discards its detailed abundance total; minimizing the grouped deviance maximizes the grouped likelihood, not the ungrouped likelihood used in the preceding score equation. The estimates therefore need not agree. The following table-based decisions use its grouped-fit convention.

## ↑ Ancestors (12)

1. [O5](../o5.md)
2. [O](../../o.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
