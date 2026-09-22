<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $h(x)=(\alpha^2+x^2)^{-1}$ and form its period-one [periodization of an integrable function](../../../../../periodization-of-an-integrable-function.md)

$$
H(x)=\sum_{k\in\mathbb Z}h(x+k).
$$

The [function](../../../../../function-split.md) $h$ is not a [Schwartz function](../../../../../schwartz-function.md), so justify the needed [Poisson summation formula](../../../../../poisson-summation-formula.md) directly. For every $j\geq0$, its [derivative](../../../../../derivative.md) satisfies $h^{(j)}(x)=O(|x|^{-2-j})$ as $|x|\to\infty$. Thus the [Weierstrass M-test](../../../../../weierstrass-m-test.md) gives [uniform convergence](../../../../../uniform-convergence.md) on $[0,1]$ of this [series](../../../../../series-mathematics.md) and each differentiated [series](../../../../../series-mathematics.md). It follows that $H$ is a [smooth](../../../../../smooth-function.md) period-one [periodic function](../../../../../periodic-function.md).

Absolute integrability and [Fubini's theorem](../../../../../fubini-s-theorem.md) allow its [Fourier coefficients](../../../../../fourier-coefficient.md) to be computed by splitting the real line into unit intervals:

$$
\begin{aligned}
b_n&=\int_0^1H(x)e^{-2\pi inx}\,dx
=\sum_k\int_k^{k+1}h(y)e^{-2\pi iny}\,dy\\
&=\widehat h(2\pi n)=\frac\pi\alpha e^{-2\pi\alpha|n|}.
\end{aligned}
$$

These [Fourier coefficients](../../../../../fourier-coefficient.md) are absolutely summable. Their [Fourier series](../../../../../fourier-series-split.md) defines a continuous [periodic function](../../../../../periodic-function.md) with the same [Fourier coefficients](../../../../../fourier-coefficient.md) as $H$; [uniqueness of Fourier coefficients in L1](../../../../../uniqueness-of-fourier-coefficients-in-l1.md) identifies the two [almost everywhere](../../../../../almost-everywhere.md), and continuity then identifies them everywhere. Evaluating at zero gives the rigorously justified [Poisson summation formula](../../../../../poisson-summation-formula.md)

$$
\frac1{\alpha^2}+2\sum_{n=1}^\infty\frac1{\alpha^2+n^2}
=H(0)=\frac\pi\alpha\left(1+2\sum_{n=1}^\infty e^{-2\pi\alpha n}\right).
$$

Rearranging proves

$$
\boxed{\sum_{n=1}^\infty\frac1{\alpha^2+n^2}
=\frac\pi{2\alpha}-\frac1{2\alpha^2}+\frac\pi\alpha\sum_{n=1}^\infty e^{-2\pi\alpha n}\qquad(\alpha>0).}
$$

The last [series](../../../../../series-mathematics.md) is a [geometric series](../../../../../geometric-series.md) with sum $(e^{2\pi\alpha}-1)^{-1}$. Equivalently, the left side is $\pi\coth(\pi\alpha)/(2\alpha)-1/(2\alpha^2)$, where $\coth$ is the [hyperbolic cotangent](../../../../../hyperbolic-cotangent.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fourier analysis course of the University of Oxford](../../../../split.md)
6. [Fourier analysis course of the University of Oxford](../../../../../fourier-analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
