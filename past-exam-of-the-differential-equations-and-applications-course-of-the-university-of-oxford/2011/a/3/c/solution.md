<h1 id="a/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $m=0$ the two normalizations agree, and the [Laguerre polynomials](../../../../../laguerre-polynomial.md) are orthonormal with weight $e^{-x}$. Take real $-1<h<1$. Their expansion coefficients for the requested function are

$$
c_n(h)=\frac1{1-h}\int_0^\infty e^{-x/(1-h)}L_n(x)\,dx.
$$

Substitute [Rodrigues' formula](../../../../../rodrigues-formula.md) and integrate by parts $n$ times. Differentiating $e^{-xh/(1-h)}$ transfers a factor $[h/(1-h)]^n$ after the two sign factors cancel. Therefore

$$
c_n(h)=\frac1{(1-h)n!}\left(\frac h{1-h}\right)^n\int_0^\infty x^ne^{-x/(1-h)}\,dx
=\boxed{h^n}.
$$

The integral is $n!(1-h)^{n+1}$ by the [Gamma function](../../../../../gamma-function.md). Boundary terms vanish throughout this range.

The resulting [generating function for Laguerre polynomials](../../../../../generating-function-for-laguerre-polynomials.md) is

$$
\boxed{\frac{e^{-xh/(1-h)}}{1-h}=\sum_{n=0}^\infty h^nL_n(x),\qquad |h|<1.}
$$

One can also verify convergence and equality directly: [Rodrigues' formula](../../../../../rodrigues-formula.md) gives $L_n(x)=\sum_{j=0}^n\binom nj(-x)^j/j!$, and summing $\sum_{n\geq j}\binom njh^n=h^j/(1-h)^{j+1}$ reduces the double series to the exponential on the left. The absolute-value double series converges for fixed $x$ and $|h|<1$, justifying the interchange; the formula then also holds for complex $h$ in that disk.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
