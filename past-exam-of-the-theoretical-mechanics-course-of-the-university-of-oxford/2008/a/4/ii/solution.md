<h1 id="a/4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Integrate once and use $h=e^{-\alpha x}$ to obtain $p'=6e^{2\alpha x}+C e^{3\alpha x}$. The two zero endpoint [pressures](../../../../../pressure-split.md) determine

$$
C=-9\frac{e^{2\alpha}-1}{e^{3\alpha}-1}=-6M,\qquad M=\frac{3(e^{2\alpha}-1)}{2(e^{3\alpha}-1)}.
$$

Consequently

$$
p'=6e^{3\alpha x}(e^{-\alpha x}-M),\qquad
p=\frac3\alpha(e^{2\alpha x}-1)-\frac{2M}\alpha(e^{3\alpha x}-1).
$$

The constant $M=\int_0^1h^{-2}\,dx/\int_0^1h^{-3}\,dx$ is a [weighted average](../../../../../weighted-arithmetic-mean.md) of $h$ with positive weight $h^{-3}$, so $e^{-\alpha}<M<1$. Since $e^{-\alpha x}$ decreases strictly, $p'$ changes sign exactly once, from positive to negative. Thus the unique maximum is at

$$
\boxed{x_m=-\frac1\alpha\log M=-\frac1\alpha\log\frac{3(e^{2\alpha}-1)}{2(e^{3\alpha}-1)}.}
$$

For small $\alpha$, $\log M=-\alpha/2-5\alpha^2/24+O(\alpha^4)$, so $\boxed{x_m=\tfrac12+\tfrac5{24}\alpha+O(\alpha^3)\sim\tfrac12}$. The [exponential-gap slider bearing](../../../../../exponential-gap-slider-bearing.md) provides a particularly simple example where a converging gap produces positive load-bearing [pressure](../../../../../pressure-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../split.md)
6. [Theoretical mechanics course of the University of Oxford](../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
