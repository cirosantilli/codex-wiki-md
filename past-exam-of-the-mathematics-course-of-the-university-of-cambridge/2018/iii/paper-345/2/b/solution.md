<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [shallow-water approximation](../../../../../../shallow-water-approximation.md), a hydrostatic vertically mixed layer, a deep motionless ambient, and no ambient [fluid entrainment](../../../../../../fluid-entrainment.md). Particle loss changes [reduced gravity](../../../../../../reduced-gravity-split.md) but changes total layer volume only at the discarded dilute-particle order. Likewise [thermal expansion](../../../../../../thermal-expansion.md) changes the [equation of state](../../../../../../equation-of-state.md) while the leading [Boussinesq approximation](../../../../../../boussinesq-approximation.md) retains [volume conservation](../../../../../../volume-conservation.md). Define

$$
b=g(\gamma\phi-\theta),\qquad D=\partial_t+u\partial_x.
$$

Depth integration of [mass conservation](../../../../../../mass-conservation.md), horizontal [momentum](../../../../../../momentum.md) balance, particle transport, and the heating law gives

$$
\boxed{\begin{aligned}
h_t+(hu)_x&=0,\\
(hu)_t+\left(hu^2+\frac12bh^2\right)_x&=0,\\
(h\phi)_t+(hu\phi)_x&=-W_s\phi,\\
(h\theta)_t+(hu\theta)_x&=\beta h\phi.
\end{aligned}}
$$

Here the integrated excess [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) is $bh^2/2$. There is no particle source from the bed. Bed drag and the particle contribution to inertia are neglected at this order. The equivalent [variable-buoyancy shallow water equations](../../../../../../variable-buoyancy-shallow-water-equations.md) are

$$
Dh=-hu_x,\qquad Du=-bh_x-\frac h2b_x,\qquad
D\phi=-\frac{W_s\phi}{h},\qquad D\theta=\beta\phi.
$$

The term $hb_x/2$ is necessary when heating or particle loss makes the [reduced gravity](../../../../../../reduced-gravity-split.md) vary horizontally.

For $v=(h,u,\phi,\theta)^T$, the [quasilinear system](../../../../../../quasilinear-system.md) $v_t+A(v)v_x=S(v)$ has

$$
A=\begin{pmatrix}
u&h&0&0\\
b&u&g\gamma h/2&-gh/2\\
0&0&u&0\\
0&0&0&u
\end{pmatrix},\qquad
S=\left(0,0,-\frac{W_s\phi}{h},\beta\phi\right)^T.
$$

Its [characteristic polynomial](../../../../../../characteristic-polynomial.md) factors as

$$
\det(A-\lambda I)=(u-\lambda)^2\bigl[(u-\lambda)^2-bh\bigr].
$$

Thus the [characteristic curves](../../../../../../characteristic-curve.md) have slopes

$$
\boxed{\frac{dx}{dt}=u-\sqrt{bh},\quad u,\quad u,\quad u+\sqrt{bh}}.
$$

On the two repeated contact [characteristic curves](../../../../../../characteristic-curve.md), the particle and heating laws are $D\phi=-W_s\phi/h$ and $D\theta=\beta\phi$. Writing $c_g=\sqrt{bh}$ and $D_\pm=\partial_t+(u\pm c_g)\partial_x$, the gravity-wave compatibility relations are

$$
D_\pm u\ \pm\frac{c_g}{h}D_\pm h=-\frac h2b_x.
$$

For $h>0$ and $b>0$, gravity-wave right [eigenvectors](../../../../../../eigenvector.md) can be taken as $(1,\pm c_g/h,0,0)^T$. The contact [eigenspace](../../../../../../eigenspace.md) has dimension two: $\delta u=0$ and $b\delta h+(h/2)\delta b=0$, with independent $\delta\phi,\delta\theta$. Therefore $A$ has a full set of real [eigenvectors](../../../../../../eigenvector.md).

**The system is hyperbolic throughout strict static stability, but not strictly hyperbolic because the contact speed is repeated.** At $b=0$ the [eigenvalues](../../../../../../eigenvalue.md) coalesce and this diagonalizability is lost; when $b<0$ the gravity-wave speeds become complex, reflecting the loss of a statically stable lower layer.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 345](../../../paper-345-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
