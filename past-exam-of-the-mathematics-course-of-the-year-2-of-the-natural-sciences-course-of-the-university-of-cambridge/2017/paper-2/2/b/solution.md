<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $d=b-a$. In the [mixed Dirichlet-Neumann problem in an elliptic annulus](../../../../../mixed-dirichlet-neumann-problem-in-an-elliptic-annulus.md), the angular [Fourier modes](../../../../../fourier-mode.md) separate. The outer data excite the $\cos\nu$ mode, while the inner derivative excites $\cos2\nu$.

For the first mode, a radial factor with zero derivative at $\mu=a$ is $\cosh(\mu-a)$. Normalizing its outer value gives $F_1(\mu)=\cosh(\mu-a)/\cosh d$. For the second mode, a radial factor vanishing at $\mu=b$ is $\sinh[2(b-\mu)]$. Its derivative at $a$ must be $-1$, fixing the coefficient to $1/[2\cosh(2d)]$. Therefore

$$
\boxed{\Phi(\mu,\nu)=\frac{\cosh(\mu-a)}{\cosh(b-a)}\cos\nu+\frac{\sinh[2(b-\mu)]}{2\cosh[2(b-a)]}\cos2\nu.}
$$

Each term satisfies [Laplace's equation](../../../../../laplace-equation.md); at $\mu=b$ the second term vanishes and the first is $\cos\nu$. At $\mu=a$, differentiating gives $0-\cos2\nu$, as required. All other modes, including the constant mode, vanish by the homogeneous mixed conditions. Alternatively, [integration by parts](../../../../../integration-by-parts.md) applied to the difference of two solutions gives a zero integral of $|\nabla\Phi|^2$, proving [uniqueness](../../../../../uniqueness.md).

**Boundary convention.** The calculation follows the explicitly printed coordinate derivative $\partial_\mu\Phi$. In [elliptic coordinates](../../../../../elliptic-coordinates.md), the [scale factor](../../../../../scale-factor-cosmology.md) is $h=\sqrt{\sinh^2\mu+\sin^2\nu}$ and the outward [unit normal](../../../../../unit-normal.md) at the inner boundary points toward decreasing $\mu$. A physical [normal derivative](../../../../../normal-derivative.md) there would be $-h^{-1}\partial_\mu\Phi$. Thus the phrase “normal derivative” in the source must be understood in its displayed coordinate sense; imposing the same numerical data on a unit-normal derivative would be a different problem.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
