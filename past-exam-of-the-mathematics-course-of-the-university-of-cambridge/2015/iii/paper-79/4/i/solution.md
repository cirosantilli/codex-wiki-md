<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use $(\bar u,\bar v)=(-\bar\psi_y,\bar\psi_x)$ and the hydrostatic [thermal-wind balance](../../../../../../thermal-wind.md) convention $\bar b=f_0\bar\psi_z$. Because the basic state is independent of $x$, $\bar v=0$. The thermal-wind relation is

$$
f_0\bar u_z=-\bar b_y=-A'(y).
$$

Integration from the resting lower boundary gives

$$
\boxed{\bar{\mathbf u}(y,z)=-\frac{zA'(y)}{f_0}\widehat{\mathbf x}.}
$$

A compatible [quasi-geostrophic streamfunction](../../../../../../quasi-geostrophic-streamfunction.md) is

$$
\bar\psi(y,z)=\frac1{f_0}\left[zA(y)+\int_0^zB(s)\,ds\right]+C,
$$

where $C$ is a spatial constant. Its horizontal [Laplacian](../../../../../../laplacian.md) is $zA''(y)/f_0$ and its second vertical derivative is $B'(z)/f_0$. Substituting into the given [three-dimensional quasi-geostrophic potential vorticity](../../../../../../three-dimensional-quasi-geostrophic-potential-vorticity.md) yields

$$
\boxed{\bar q=f_0+\frac{zA''(y)}{f_0}+\frac{f_0}{N^2}B'(z).}
$$

In particular, the horizontal-curvature term has a plus sign: $\bar\zeta=-\bar u_y=zA''/f_0$.

The [reference-buoyancy convention in quasi-geostrophic potential vorticity](../../../../../../reference-buoyancy-convention-in-quasi-geostrophic-potential-vorticity.md) should be stated. If $\bar b$ includes the full reference profile $N^2z$, the formula above includes its constant contribution $f_0$. If instead the [quasi-geostrophic streamfunction](../../../../../../quasi-geostrophic-streamfunction.md) represents pressure relative to that reference hydrostatic state, use $\bar b-N^2z=f_0\bar\psi_z$. Then the quoted $\bar q$ is reduced by the constant $f_0$. Both conventions give exactly the same velocity and [potential-vorticity gradients](../../../../../../potential-vorticity-gradient.md), and therefore the same subsequent dynamics. The coefficient $N$ in the stated linear model is a prescribed reference [buoyancy frequency](../../../../../../buoyancy-frequency.md); if it is also required to equal the full physical buoyancy frequency everywhere, then $B'(z)=N^2$, rather than an arbitrary function. The formal expression above retains the requested arbitrary $B$ with the stated constant coefficient.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
