<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Choose equation (1), evaluated by refined composite [Simpson's rule](../../../../../simpson-s-rule.md).** It gives $y$ directly as a one-dimensional [definite integral](../../../../../definite-integral.md) with fixed endpoints and a smooth integrand. It therefore avoids [root finding](../../../../../root-finding.md) altogether. Before evaluating, use the [trigonometric identity](../../../../../trigonometric-identity.md)

$$
\sin(x-a\cos x)+\sin(x+a\cos x)=2\sin x\cos(a\cos x),\qquad a=\pi/4.
$$

This equivalent integrand is nonnegative throughout $[0,\pi/2]$, avoiding cancellation between the original two terms. Equation (2) instead subtracts two potentially large [exponential functions](../../../../../exponential-function.md), while equation (3) would ordinarily put a [numerical integration](../../../../../numerical-integration-split.md) inside a [root finding](../../../../../root-finding.md) loop.

For even $n$, let $h=(\pi/2)/n$, $\phi(x)=2\sin x\cos((\pi/4)\cos x)$, and compute

$$
Y_n=\frac\pi4\frac h3\left[\phi(0)+\phi(\pi/2)+4\sum_{\substack{1\leq j<n\\j\text{ odd}}}\phi(jh)+2\sum_{\substack{2\leq j<n\\j\text{ even}}}\phi(jh)\right].
$$

Then double $n$. The integrand has bounded [derivatives](../../../../../derivative.md) of every fixed order on the integration [interval](../../../../../interval-mathematics.md); in the fourth-order error regime, the estimated remaining [truncation error](../../../../../truncation-error.md) in $Y_{2n}$ is $|Y_{2n}-Y_n|/15$. The factor $15$ follows by eliminating the leading term $Ch^4$ between the two mesh widths.[§3.5(ii), composite rule and error, equations 3.5.6–3.5.8](../../../../../nist-digital-library-of-mathematical-functions/3-5-quadrature-subsection-ii-simpson%E2%80%99s-rule.md)

**Stop when this estimate is comparable to $\varepsilon_{\rm mach}\max(1,|Y_{2n}|)$ and further refinement shows stagnation at the [roundoff error](../../../../../round-off-error.md) scale.** Check that the differences previously decreased consistently with fourth-order [convergence](../../../../../convergence.md); differences alone are not a rigorous error certificate if cancellation or [roundoff error](../../../../../round-off-error.md) dominates. [Compensated summation](../../../../../compensated-summation.md) helps keep the summation error near the precision limit. Refining indefinitely after this point increases work without reliably adding meaningful digits. This answers the requested choice and termination strategy without requiring an explicit value of $y$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Discrete mathematics, continuous mathematics, and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
