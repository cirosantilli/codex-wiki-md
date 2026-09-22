<h1 id="o5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The unrestricted likelihood is maximized at the empirical proportions, while the null likelihood is maximized at $\pi_i(\widehat\theta)$. Twice the log of their ratio is

$$
\boxed{\Lambda(\widehat\theta)=2\sum_i n_i\log\frac{n_i}{n\pi_i(\widehat\theta)}.}
$$

Large values mean the fitted null likelihood is much smaller than the unrestricted maximum, so rejection is in the upper tail.

For a regular identifiable scalar parameter lying in the interior, positive true cell probabilities, and sufficiently large expected counts, [Wilks theorem](../../../../wilks-theorem.md) gives an approximate [chi-squared distribution](../../../../chi-squared-distribution.md) with $(k-1)-1=k-2$ degrees of freedom under the null. The unrestricted [probability](../../../../probability.md) [vector](../../../../vector.md) has dimension $k-1$ and the fitted null has dimension one. At significance level $\alpha$, reject if $\Lambda(\widehat\theta)>F_{k-2}^{-1}(1-\alpha)$, or report the approximate p-value $1-F_{k-2}(\Lambda)$.

Cells with very small expected counts may require a prespecified pooling scheme or simulation calibration; the asymptotic reference is not an exact finite-sample law. For a regular null with $d$ fitted parameters, the corresponding degrees of freedom are $k-1-d$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [O5](../../o5.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
