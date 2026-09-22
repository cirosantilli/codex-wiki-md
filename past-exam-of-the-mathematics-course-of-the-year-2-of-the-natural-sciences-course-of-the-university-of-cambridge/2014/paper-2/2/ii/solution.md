<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Resolve the angular [surface charge density](../../../../../surface-charge-density.md) into [Legendre polynomials](../../../../../legendre-polynomial.md):

$$
\sin^2\theta=\frac23[1-P_2(\cos\theta)],\qquad \sigma_0=\frac{2A}{3},\quad\sigma_2=-\frac{2A}{3}.
$$

For a single degree $\ell$, write the common surface potential as $V_\ell P_\ell$. Regularity and decay require radial factors $(r/R)^\ell$ inside and $(R/r)^{\ell+1}$ outside. Their exterior-minus-interior radial derivative at $R$ is $-(2\ell+1)V_\ell P_\ell/R$. Thus [spherical harmonic matching with a derivative jump](../../../../../spherical-harmonic-matching-with-a-derivative-jump.md) gives $V_\ell=R\sigma_\ell/(2\ell+1)$.

Only degrees zero and two occur, yielding

$$
\boxed{\begin{aligned}
\Psi_{\rm in}(r,\theta)&=\frac{2AR}{3}-\frac{2A}{15R}r^2P_2(\cos\theta),&&r<R,\\
\Psi_{\rm out}(r,\theta)&=\frac{2AR^2}{3r}-\frac{2AR^4}{15r^3}P_2(\cos\theta),&&r>R.
\end{aligned}}
$$

Both expressions have surface value $2AR/3-2AR P_2/15$, and their derivative difference is $-2A/3+(2A/3)P_2=-A\sin^2\theta$, checking both interface conditions. The interior quadratic is regular at the origin, and the exterior potential tends to zero.

The leading far-field term is the monopole term. Indeed the total charge is $Q=R^2\int\sigma\,d\Omega=8\pi AR^2/3$, and the normalization of the specified jump gives $Q/(4\pi r)=2AR^2/(3r)$. No extra permittivity factor is inserted into the supplied normalization. Regularity here means finite piecewise smooth potential; its normal derivative necessarily jumps at the charged surface.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
