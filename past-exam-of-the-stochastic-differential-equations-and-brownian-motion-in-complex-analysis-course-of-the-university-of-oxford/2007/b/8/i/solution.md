<h1 id="b/8/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The printed upper-tail identity cannot be a probability formula: it vanishes at zero and increases in $x$. Its correction is

$$
\boxed{\mathbb P_i(X_{T_{\mathbb H}}>x)=\tfrac12-\frac1\pi\arctan x.}
$$

Equivalently the cumulative distribution function is $1/2+\pi^{-1}\arctan x$. Differentiating that cumulative function gives the density

$$
\frac1{\pi(1+x^2)}.
$$

The normalization and sign can also be checked directly by [conformal invariance of planar Brownian motion](../../../../../conformal-invariance-of-planar-brownian-motion.md): the [Cayley transform](../../../../../cayley-transform-complex-analysis.md) $(z-i)/(z+i)$ sends the starting point to the center of the [unit disc](../../../../../unit-disc.md). Its exit angle is uniform by rotational symmetry. The inverse on the [unit circle](../../../../../complex-unit-circle.md) gives $X=-\cot(\Theta/2)$, $\Theta$ uniform on $(0,2\pi)$, whose change-of-variable density is exactly the one above.

For a start $z_0=x_0+iy_0$, $y_0>0$, translation and positive scaling send it to $i$. Thus the exit coordinate has law $x_0+y_0C$, where $C$ is standard Cauchy. The corresponding formulas are

$$
\boxed{\mathbb P_{z_0}(X_{T_{\mathbb H}}\in ds)
=\frac{y_0\,ds}{\pi((s-x_0)^2+y_0^2)},\quad
\mathbb P_{z_0}(X_{T_{\mathbb H}}>a)
=\frac12-\frac1\pi\arctan\frac{a-x_0}{y_0}.}
$$

This is the upper-half-plane [Poisson kernel](../../../../../poisson-kernel.md). The printed density is correct; it is the preceding asserted tail from which it is meant to follow that needs correction.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
