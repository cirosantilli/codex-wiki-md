<h1 id="7/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the upper [Apollonius circle](../../../../../../circles-of-apollonius.md), let its constant ratio be $P>1$. Matching the center and radius from part (i) gives

$$
y_0=\frac{b(P^2+1)}{P^2-1},\qquad R=\frac{2bP}{P^2-1}.
$$

Subtracting their squares yields $\boxed{b=\sqrt{y_0^2-R^2}}$. Also

$$
\frac{y_0}{R}=\frac{P+P^{-1}}2=\cosh(\log P),\qquad\log P=\operatorname{arcosh}(y_0/R).
$$

The relevant [inverse hyperbolic cosine](../../../../../../inverse-hyperbolic-cosine.md) is positive. Now $\log|(z+ib)/(z-ib)|$ is the [real part](../../../../../../real-part.md) of a local [holomorphic logarithm](../../../../../../holomorphic-logarithm.md), hence a [harmonic function](../../../../../../harmonic-function.md) away from $z=\pm ib$. The point $ib$ is inside the excluded disk, because $0<y_0-b<R$, while $-ib$ is below the real axis. Thus neither singularity lies in the physical domain.

On $y=0$ the numerator and denominator have equal [modulus](../../../../../../modulus.md), so the logarithm is zero. On the circular boundary its value is $\log P=\operatorname{arcosh}(y_0/R)$. Therefore the [harmonic potential between a grounded line and a circular boundary](../../../../../../harmonic-potential-between-a-grounded-line-and-a-circular-boundary.md) is

$$
\boxed{V(x,y)=\frac{V_0}{\operatorname{arcosh}(y_0/R)}\log\left|\frac{x+iy+i\sqrt{y_0^2-R^2}}{x+iy-i\sqrt{y_0^2-R^2}}\right|.}
$$

This verifies [Laplace's equation](../../../../../../laplace-equation.md) and both prescribed [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md). It also tends to zero at infinity. A uniqueness assertion on this unbounded domain would require an additional boundedness or infinity condition; the displayed function is the natural decaying solution requested.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
