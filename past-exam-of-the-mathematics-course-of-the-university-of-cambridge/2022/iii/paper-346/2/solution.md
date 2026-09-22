<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The two halo centres orbit their [centre of mass](../../../../../center-of-mass.md) with separation $R$. Their relative coordinate obeys $\ddot{\mathbf R}=-G(M_1+M_2)\mathbf R/R^3$, hence circular motion requires

$$
\boxed{\omega^2=\frac{G(M_1+M_2)}{R^3}.}
$$

Reflection symmetry about the orbital plane makes the vertical force point back toward $z=0$, while the centrifugal force has no vertical component. An equilibrium away from that plane is therefore impossible.

In the uniformly rotating frame, an equilibrium is a stationary point of the gravitational plus centrifugal [effective potential](../../../../../effective-potential.md)

$$
E(x,y)=-\frac{\omega^2}{2}|\mathbf r_S|^2
-\frac{GM_1}{|\mathbf r_S-\mathbf r_1|}
-\frac{GM_2}{|\mathbf r_S-\mathbf r_2|}.
$$

Set $R=1$, divide by $G(M_1+M_2)/R$, and write $\alpha=M_2/(M_1+M_2)$. The primary and secondary lie at $x=-\alpha$ and $x=1-\alpha$, so on their line

$$
F(x)=-\frac{x^2}{2}-\frac{1-\alpha}{|x+\alpha|}
-\frac\alpha{|x+\alpha-1|}.
$$

For the two roots near the secondary, put $x=1-\alpha\mp d$ in $F'(x)=0$. Dominant balance gives $3d\simeq\alpha/d^2$, so $d=(\alpha/3)^{1/3}$. Expanding the root beyond the primary directly in powers of $\alpha$ gives

$$
\boxed{L_1=(1-(\alpha/3)^{1/3},0,0),}
$$



$$
\boxed{L_2=(1+(\alpha/3)^{1/3},0,0),}
$$



$$
\boxed{L_3=(-1-5\alpha/12,0,0),}
$$

to the requested orders. The other equilibria are the two [Triangular Lagrange points](../../../../../triangular-lagrange-point.md)

$$
\boxed{L_{4,5}=(1/2-\alpha,\ \pm\sqrt3/2,\ 0).}
$$

The distance from $H_2$ to either nearby collinear point is the [Hill radius](../../../../../hill-radius.md). Since $\alpha\simeq M_2/M_1$,

$$
\boxed{r_t=R\left(\frac{M_2}{3M_1}\right)^{1/3}.}
$$

Inside this [tidal radius](../../../../../tidal-radius.md), the subhalo's gravity dominates the host's differential gravitational field; outside it, material can escape through the neighborhoods of $L_1$ and $L_2$. For an extended spherical host, $M_1$ is replaced by enclosed mass and the coefficient becomes $3-d\log M_1/d\log R$, giving the [Jacobi tidal radius](../../../../../jacobi-tidal-radius.md). An extended subhalo requires the bound mass inside $r_t$ to be found self-consistently. On an eccentric orbit there is no time-independent rotating potential or exact tidal boundary; stripping is strongest near pericentre and the instantaneous radius varies around the orbit.

Because the dark component is more extended, [tidal stripping](../../../../../tidal-stripping.md) first sends dark matter through both $L_1$ and $L_2$, producing leading and trailing dark-matter [tidal tails](../../../../../tidal-tail.md). The compact stellar component is stripped more deeply and also produces a leading and a trailing stellar tail. The two constituents therefore give four tails distinguished by composition, with the dark tails broader and more extended.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 346](../../paper-346-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
