<h1 id="a/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the valid [Gaussian maximum](../../../../../gaussian-maximum.md) estimate from part (b), with

$$
a_n=\sqrt{2(n+1)\log2}>1.
$$

Split the [tail integral formula for expectation](../../../../../tail-integral-formula-for-expectation.md) at $a_n$. Bounding the first part by $a_n$ and applying the Gaussian tail estimate to the second gives

$$
\mathbb E M_n
\leq a_n+C_n\int_{a_n}^\infty e^{-x^2/2}\,dx
\leq a_n+\frac{C_n}{a_n}e^{-a_n^2/2}
=a_n+\frac1{\sqrt{2\pi}\,a_n}.
$$

Thus $\mathbb E M_n=O(\sqrt n)$. The finitely many small indices also have finite expectation; the bound above already covers them.

By [Tonelli's theorem](../../../../../tonelli-theorem.md), nonnegativity permits interchanging sum and expectation:

$$
\boxed{\mathbb E\left[\sum_{n\geq1}2^{-n/2}M_n\right]
=\sum_{n\geq1}2^{-n/2}\mathbb E M_n<\infty.}
$$

The final series converges because its exponential decay dominates the factor $\sqrt n$. This establishes the requested conclusion independently of the false bound printed in (1).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
