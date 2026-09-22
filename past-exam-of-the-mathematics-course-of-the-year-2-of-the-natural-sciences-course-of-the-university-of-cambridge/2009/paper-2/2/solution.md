<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Set $\Phi=R(r)P(\theta)$ and multiply the [Laplace equation](../../../../laplace-equation.md) by $r^2/(RP)$. [Separation of variables](../../../../separation-of-variables.md) gives

$$
\frac{(r^2R')'}R=-\frac{(\sin\theta P')'}{\sin\theta P}=\lambda.
$$

With $\xi=\cos\theta$, the angular equation is $[(1-\xi^2)P_\xi]' +\lambda P=0$. Regularity at both poles selects the [Legendre polynomials](../../../../legendre-polynomial.md) $P_n$ and $\lambda=n(n+1)$. The radial [Cauchy-Euler equation](../../../../cauchy-euler-equation.md) has solutions $r^n,r^{-n-1}$. Expanding the angular data in this complete orthogonal system therefore gives

$$
\Phi(r,\theta)=\sum_{n=0}^\infty(A_nr^n+B_nr^{-n-1})P_n(\cos\theta),
$$

with the usual convergence required of a [harmonic](../../../../harmonic-function.md) expansion on the region considered. Angular Legendre functions singular at the poles are excluded.

For $0<a<b$, the outer data have expansion $b^2\cos^2\theta=b^2/3+(2b^2/3)P_2(\cos\theta)$, while the inner data are pure $P_0$. Thus only degrees zero and two are needed. A radial interpolation matching each pair of boundary values gives

$$
\boxed{\Phi(r,\theta)=\frac{a^3(b-r)+(b^3/3)(r-a)}{r(b-a)}
+\frac{2b^2}{3}\frac{r^2-a^5/r^3}{b^2-a^5/b^3}P_2(\cos\theta).}
$$

The first term is a [linear combination](../../../../linear-combination.md) of $1,r^{-1}$ and takes values $a^2,b^2/3$ at the two radii. The second is a combination of $r^2,r^{-3}$ and takes values zero and $2b^2/3$. These checks establish both boundary conditions; each term is [harmonic](../../../../harmonic-function.md). The [maximum principle for harmonic functions](../../../../maximum-principle-for-harmonic-functions.md) gives uniqueness. This is an example of [axisymmetric harmonic interpolation between concentric spheres](../../../../axisymmetric-harmonic-interpolation-between-concentric-spheres.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper 2](../../paper-2-split.md)
3. [2009](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
