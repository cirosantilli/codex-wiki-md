<h1 id="14d/solution">Solution</h1>

↑ **Parent:** [14D](../14d.md)

The intended open region lies inside the larger circle and outside the smaller one. The two circles are tangent at zero, a boundary point, so $w=1/z$ is holomorphic throughout the region. For a circle $|z-ia|=a$, its equation is $|z|^2=2a\operatorname{Im}z$, which becomes $\operatorname{Im}w=-1/(2a)$. The side inside that circle becomes $\operatorname{Im}w<-1/(2a)$. Hence the [tangent-circle crescent conformal map](../../../../../tangent-circle-crescent-conformal-map.md) begins with

$$
\Omega\longrightarrow\left\{w:-\frac12<\operatorname{Im}w<-\frac14\right\},\qquad w=\frac1z.
$$

The affine coordinate $\zeta=4w+2i$ sends this strip bijectively to $0<\operatorname{Im}\zeta<1$. Exponentiation $\eta=e^{\pi\zeta}$ is then a conformal bijection to the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md): its argument ranges strictly from zero to $\pi$, and the inverse logarithm has that unique argument. Finally $(\eta-i)/(\eta+i)$ is a [Cayley transform between the half-plane and disk](../../../../../cayley-transform-between-the-half-plane-and-disk.md) onto the [unit disc](../../../../../unit-disc.md), since for $\operatorname{Im}\eta>0$ its modulus is less than one and the inverse is $\eta=i(1+u)/(1-u)$. As $e^{\pi\zeta}=e^{4\pi/z}$, a complete answer is

$$
\boxed{F(z)=\frac{e^{4\pi/z}-i}{e^{4\pi/z}+i}.}
$$

Every stage has nonzero derivative and is one-to-one onto its indicated range. The denominator cannot vanish in the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md). Unlike a region between disjoint nested circles, this tangent crescent has no enclosed hole, so there is no annulus obstruction to mapping it onto a disc.

## ↑ Ancestors (10)

1. [14D](../14d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
