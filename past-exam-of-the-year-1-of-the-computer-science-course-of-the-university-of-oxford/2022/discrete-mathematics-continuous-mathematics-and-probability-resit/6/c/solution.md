<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $h=(b-a)/n$ and let $M_4=\max_{x\in[a,b]}|f^{(4)}(x)|$. A [composite Simpson's rule](../../../../../composite-simpson-s-rule.md) panel covers two strips, so it has width $2h$ and absolute error at most

$$
\frac{(2h)^5}{2880}M_4=\frac{h^5}{90}M_4.
$$

There are $n/2$ panels. By the [triangle inequality](../../../../../triangle-inequality.md), the absolute error of their sum is at most the sum of their absolute errors. Hence

$$
\boxed{|I-S_n|\leq\frac n2\frac{h^5}{90}M_4
=\frac{(b-a)^5}{180n^4}M_4.}
$$

This assumes even $n$ and, for the usual Simpson remainder theorem, $f\in C^4[a,b]$. In particular its fourth [derivative](../../../../../derivative.md) is bounded on the interval. It is the [error bound for composite Simpson's rule](../../../../../error-bound-for-composite-simpson-s-rule.md), expressed in strip count rather than panel count.[NIST DLMF §3.5(ii), equations 3.5.6–3.5.8: elementary and composite Simpson error terms](../../../../../nist-digital-library-of-mathematical-functions/3-5-quadrature-subsection-ii-simpson%E2%80%99s-rule.md)

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Discrete mathematics, continuous mathematics and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
