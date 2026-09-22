<h1 id="4/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $n$ to be a positive even integer, as required by [composite Simpson's rule](../../../../../../composite-simpson-s-rule.md). There are $n/2$ two-strip panels, each of width $2/n$. Applying the supplied panel bound with the global fourth-[derivative](../../../../../../derivative.md) minimum $0$ and maximum $1$, and summing, gives

$$
\boxed{0\le E_n\le\frac{n}{2}\frac{(2/n)^5}{2880}
=\frac1{180n^4}.}
$$

Here $E_n$ is the nonnegative [absolute error](../../../../../../absolute-error.md). In this example [Simpson's rule](../../../../../../simpson-s-rule.md) overestimates the [integral](../../../../../../integral-split.md), so $E_n=S_n-I$. Each panel has that same sign because its fourth [derivative](../../../../../../derivative.md) is nonnegative; cancellation is not being assumed.[§3.5(ii), equations 3.5.6–3.5.8: elementary and composite fourth-[derivative](../../../../../../derivative.md) remainders](../../../../../../nist-digital-library-of-mathematical-functions/3-5-quadrature-subsection-ii-simpson%E2%80%99s-rule.md)

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
