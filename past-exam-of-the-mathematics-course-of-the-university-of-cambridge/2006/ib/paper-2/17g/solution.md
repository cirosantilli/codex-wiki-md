<h1 id="17g/solution">Solution</h1>

↑ **Parent:** [17G](../17g.md)

For steady [electromagnetic fields](../../../../../electromagnetic-field.md), [Maxwell's equations](../../../../../maxwell-equations.md) give $\nabla\times\boldsymbol B=\mu_0\boldsymbol j$ and $\nabla\cdot\boldsymbol B=0$. Introduce a [magnetic vector potential](../../../../../magnetic-vector-potential.md) with $\boldsymbol B=\nabla\times\boldsymbol A$ and the permitted [Coulomb gauge](../../../../../coulomb-gauge.md) $\nabla\cdot\boldsymbol A=0$. The vector identity for the double curl then gives $-\Delta\boldsymbol A=\mu_0\boldsymbol j$. For localized currents and the decaying solution,

$$
\boldsymbol A(\boldsymbol r)=\frac{\mu_0}{4\pi}\int_V\frac{\boldsymbol j(\boldsymbol r')}{|\boldsymbol r-\boldsymbol r'|}dV'.
$$

Here $-\Delta(1/(4\pi|\boldsymbol r|))=\delta$ follows from harmonicity away from zero and the inward flux of the radial derivative through a small sphere, whose magnitude is one. It verifies the vector Poisson solution componentwise. Moreover steady [electric charge conservation](../../../../../charge-conservation.md) gives $\nabla'\cdot\boldsymbol j=0$; integration by parts confirms the stated potential is divergence-free. Taking its curl, using $\nabla |\boldsymbol r-\boldsymbol r'|^{-1}=-(\boldsymbol r-\boldsymbol r')/|\boldsymbol r-\boldsymbol r'|^3$, proves the [Biot-Savart law](../../../../../biot-savart-law.md):

$$
\boxed{\boldsymbol B(\boldsymbol r)=\frac{\mu_0}{4\pi}\int_V\frac{\boldsymbol j(\boldsymbol r')\times(\boldsymbol r-\boldsymbol r')}{|\boldsymbol r-\boldsymbol r'|^3}dV'.}
$$

The zero-field condition at infinity selects the [magnetic field](../../../../../magnetic-field.md) produced by these currents, excluding an externally imposed homogeneous [magnetic field](../../../../../magnetic-field.md).

At the origin write the source point as $r\boldsymbol e_r+z\boldsymbol e_z$. Its current is $kr\boldsymbol e_\phi$, so the numerator of the [Biot-Savart law](../../../../../biot-savart-law.md) is $kr^2\boldsymbol e_z-krz\boldsymbol e_r$. The radial term cancels after angular integration. Using $dV'=r\,dr\,d\phi\,dz$ gives

$$
B_z(0)=\frac{\mu_0k}{2}\int_0^b r^3dr\int_{-h}^h\frac{dz}{(r^2+z^2)^{3/2}}.
$$

The inner [integral](../../../../../integral.md) is $2h/[r^2\sqrt{h^2+r^2}]$, as is verified by differentiating $z/[r^2\sqrt{r^2+z^2}]$. Hence

$$
\boxed{\boldsymbol B(0)=\mu_0kh\left(\sqrt{h^2+b^2}-h\right)\boldsymbol e_z.}
$$

For $b,h>0$, its magnitude is $\mu_0|k|h(\sqrt{h^2+b^2}-h)$; it points along $+z$ for positive azimuthal current $k>0$, and along $-z$ for $k<0$. The limit $h\to\infty$ is $\mu_0kb^2/2$, agreeing with direct integration of the infinitely long cylindrical current distribution.

## ↑ Ancestors (10)

1. [17G](../17g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
