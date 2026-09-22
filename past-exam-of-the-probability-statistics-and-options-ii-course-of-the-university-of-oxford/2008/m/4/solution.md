<h1 id="m/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The moment generating function is $M_X(t)=\mathbb E(e^{tX})$ wherever that [expectation](../../../../expected-value-split.md) is finite. A useful [continuity](../../../../continuous-function.md) theorem says that if the moment generating functions $M_n$ are finite on a common [open interval](../../../../open-interval.md) containing zero and converge pointwise there to the moment generating function of a probability distribution, then the corresponding variables converge in distribution to that law. Equivalently one may assume a finite limiting function on such a neighborhood, with the usual [continuity](../../../../continuous-function.md) at zero, and obtain the uniquely determined limiting law.

For the gamma density, integrating the exponential against the density and changing variable to $(\lambda-t)x$ gives

$$
\boxed{M_X(t)=\left(\frac\lambda{\lambda-t}\right)^\alpha,\qquad t<\lambda.}
$$

For the waiting time to one head, [independence](../../../../independent-random-variables.md) of successive tosses gives $\Pr(Y=j)=p(1-p)^{j-1}$ for $j\ge1$. Summing the [geometric series](../../../../geometric-series.md) gives

$$
\boxed{M_Y(t)=\frac{pe^t}{1-(1-p)e^t},\qquad (1-p)e^t<1.}
$$

The waiting times between consecutive heads are [independent](../../../../independent-random-variables.md) copies of $Y$, so their sum $N$ has moment generating function $M_Y(t)^k$. Consequently

$$
M_{2pN}(t)=\left[\frac{pe^{2pt}}{1-(1-p)e^{2pt}}\right]^k\longrightarrow(1-2t)^{-k}.
$$

For fixed $t<1/2$, numerator and denominator have leading terms $p$ and $p(1-2t)$ as $p\downarrow0$. A fixed neighborhood of zero is inside the convergence domain for all sufficiently small $p$, so the [continuity](../../../../continuous-function.md) theorem applies. The limiting distribution is

$$
\boxed{\operatorname{Gamma}(\text{shape }k,\ \text{rate }1/2),}
$$

equivalently a [chi-squared distribution](../../../../chi-squared-distribution.md) with $2k$ [degrees of freedom](../../../../degree-of-freedom.md).

## ↑ Ancestors (12)

1. [4](../4.md)
2. [M](../../m.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
