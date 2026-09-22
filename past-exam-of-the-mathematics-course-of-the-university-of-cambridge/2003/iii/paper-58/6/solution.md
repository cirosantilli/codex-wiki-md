<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Normalize a point source by $\int\rho\,d^3x\,dz=q_1$ on the compact spatial direction. The periodic delta has the [Fourier series](../../../../../fourier-series-split.md)

$$
\delta_{2\pi R}(z)=\frac1{2\pi R}\sum_{n\in\mathbb Z}e^{inz/R}.
$$

Writing the potential as $\phi(r,z)=\sum_n\phi_n(r)e^{inz/R}$ reduces the [Poisson equation](../../../../../poisson-equation.md) to

$$
\left(\nabla_3^2-\frac{n^2}{R^2}\right)\phi_n=-2q_1\delta^3(\mathbf x).
$$

Away from the source, the decaying radial solution is proportional to $e^{-|n|r/R}/r$. Its distributional normalization follows from integrating the Laplacian over a small sphere: the radial flux of $1/r$ is $-4\pi$, so

$$
\phi_n(r)=\frac{q_1}{2\pi r}e^{-|n|r/R}.
$$

This is the contribution of the $n$th [Kaluza-Klein mode](../../../../../kaluza-klein-mode.md), with inverse range $|n|/R$. At equal compact coordinate, the sum is a geometric series,

$$
\phi(r,0)=\frac{q_1}{2\pi r}\left(1+2\sum_{n=1}^\infty e^{-nr/R}\right)
=\frac{q_1}{2\pi r}\coth\frac{r}{2R}.
$$

Therefore the pair interaction energy, without the individual self-energies, is

$$
\boxed{U(r)=\frac{q_1q_2}{2\pi r}\coth\frac{r}{2R}.}
$$

Its normalization is fixed by the stated $-4\pi R\rho$ source, rather than by importing another convention for [Coulomb's law](../../../../../coulomb-s-law.md). More generally summing the phases gives the [periodic electrostatic Green function with one compact dimension](../../../../../periodic-electrostatic-green-function-with-one-compact-dimension.md),

$$
\phi(r,z)=\frac{q_1}{2\pi r}\frac{\sinh(r/R)}{\cosh(r/R)-\cos(z/R)}.
$$

An independent check uses the [method of images](../../../../../method-of-images.md) in four spatial dimensions. Since $\nabla_4^2s^{-2}=-4\pi^2\delta^4$, its periodic image sum is $Rq_1\sum_n[r^2+(z+2\pi nR)^2]^{-1}/\pi$, with the same normalization and short-distance singularity.

For $r\gg R$, only the zero [Kaluza-Klein mode](../../../../../kaluza-klein-mode.md) survives:

$$
\boxed{U(r)=\frac{q_1q_2}{2\pi r}\left[1+2e^{-r/R}+O(e^{-2r/R})\right].}
$$

For $r\ll R$, $\coth x=x^{-1}+x/3+O(x^3)$ gives

$$
\boxed{U(r)=\frac{q_1q_2R}{\pi r^2}+\frac{q_1q_2}{12\pi R}+O(r^2/R^3).}
$$

The leading potential thus changes from inverse distance to inverse squared distance. Differentiating gives the signed outward force

$$
F_r=\frac{q_1q_2}{2\pi}\left[\frac{\coth(r/(2R))}{r^2}
+\frac{\operatorname{csch}^2(r/(2R))}{2Rr}\right].
$$

It scales as $r^{-2}$ at large distance and as $2q_1q_2R/(\pi r^3)$ at small distance. **A precision inverse-square-law test over separations approaching $R$ would reveal the extra dimension** through this change of force law or its exponential corrections. The model assumes localized sources at equal compact coordinate and an electromagnetic field able to explore the circle; a field confined to ordinary spacetime would not show this effect. Finite source size and ordinary screening must be controlled when comparing a real force measurement with this point-source prediction.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
