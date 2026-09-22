<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Projection onto the constant [polynomials](../../../../polynomial-split.md) requires the residual to be [orthogonal](../../../../orthogonal-vectors.md) to $1$. For the original [inner product](../../../../inner-product-split.md),

$$
0=\int_{-1}^1(x^2-p_0)\,dx=\frac23-2p_0,\qquad \boxed{p_0=\frac13.}
$$

For the weighted [inner product](../../../../inner-product-split.md) the corresponding [normal equation](../../../../normal-equation.md) is

$$
0=\int_{-1}^1x^{2n}(x^2-\bar p_0(n))\,dx=\frac2{2n+3}-\bar p_0(n)\frac2{2n+1}.
$$

Hence

$$
\boxed{\bar p_0(n)=\frac{2n+1}{2n+3}=1-\frac2{2n+3}\longrightarrow1.}
$$

It increases monotonically towards one. Although the weight vanishes at zero, it is positive elsewhere, and a nonzero continuous function is nonzero on an interval of positive weight. Thus the weighted expression really is an [inner product](../../../../inner-product-split.md) and the constant minimizer is unique.

The normalized weight $(2n+1)x^{2n}/2$ has total mass one and assigns mass $r^{2n+1}$ to $[-r,r]$ for each $0<r<1$. Its mass therefore concentrates near $-1$ and $1$, where $x^2=1$. This explains why the weighted best constant tends to one rather than to the unweighted spatial average. It is [endpoint concentration in weighted constant approximation](../../../../endpoint-concentration-in-weighted-constant-approximation.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
