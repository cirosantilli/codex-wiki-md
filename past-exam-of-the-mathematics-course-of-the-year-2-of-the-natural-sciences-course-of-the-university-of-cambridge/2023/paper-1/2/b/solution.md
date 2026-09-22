<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The two homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) on $x$ force negative separation constants. The initial profile is an [even function](../../../../../even-function.md), so only the even sine-family [eigenfunctions](../../../../../eigenfunction.md) are needed:

$$
X_m(x)=\cos(k_mx),\qquad k_m=\left(m+\frac12\right)\pi,\qquad m=0,1,\ldots.
$$

They obey $X_m(\pm1)=0$ and $\int_{-1}^1X_mX_n\,dx=\delta_{mn}$. Odd [eigenfunctions](../../../../../eigenfunction.md) have zero projection onto the even initial data. Hence the initial coefficients are

$$
\begin{aligned}
a_m&=\int_{-1}^1(1-x^2)\cos(k_mx)\,dx\\
&=2\left[-\frac{2x\cos(k_mx)}{k_m^2}+\frac{2\sin(k_mx)}{k_m^3}\right]_0^1
=\frac{4(-1)^m}{k_m^3}.
\end{aligned}
$$

The desired [eigenfunction expansion](../../../../../eigenfunction-expansion.md) is therefore

$$
\boxed{u(x,y)=4\sum_{m=0}^{\infty}\frac{(-1)^m}{k_m^3}\cos(k_mx)\exp[-(k_m^2+1)y+\cos y-1],\qquad k_m=(m+\tfrac12)\pi.}
$$

At $y=0$ this is the [Fourier series](../../../../../fourier-series-split.md) of $1-x^2$ on the interval; its coefficients are absolutely summable. Each term satisfies the [partial differential equation](../../../../../partial-differential-equation-split.md) and side conditions. For $y>0$ the additional Gaussian decay in $m$ justifies termwise [differentiation](../../../../../differentiation.md). Since $k_m^2+1>0$ and $e^{\cos y-1}\leq1$, the whole series decays uniformly as $y\to\infty$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
