<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $u=\Re f$, and suppose $u$ has a local maximum at $z_0\in U$. Choose $R>0$ such that the closed disk $\overline{D(z_0,R)}$ lies in $U$ and $u(z)\leq u(z_0)$ throughout it. Start [planar Brownian motion](../../../../../../../planar-brownian-motion.md) $B$ at $z_0$, and for $0<r<R$ let $\tau_r$ be its first exit from $D(z_0,r)$.

By part (a) and [Itô formula](../../../../../../../ito-s-lemma.md), $u(B_{t\wedge\tau_r})$ is a [local martingale](../../../../../../../local-martingale.md); boundedness of $u$ on the compact disk makes it a true bounded [martingale](../../../../../../../martingale-split.md). The exit time is finite [almost surely](../../../../../../../almost-sure-convergence.md). One direct check applies the same formula to $|B_{t\wedge\tau_r}-z_0|^2$, giving $2\mathbb E(t\wedge\tau_r)=\mathbb E|B_{t\wedge\tau_r}-z_0|^2\leq r^2$. Thus $\mathbb E\tau_r\leq r^2/2$.

The [optional stopping theorem](../../../../../../../optional-sampling-theorem-for-a-supermartingale.md), first at $t\wedge\tau_r$ and then by bounded convergence, gives

$$
u(z_0)=\mathbb E_{z_0}u(B_{\tau_r}).
$$

The exit point is uniformly distributed on the circle: [rotational invariance of planar Brownian motion](../../../../../../../rotational-invariance-of-planar-brownian-motion.md) about its starting point makes its exit law rotation invariant, and normalized arc length is the unique rotation-invariant probability measure on a circle. Since every boundary value is at most $u(z_0)$, equality of the mean forces every boundary value to equal $u(z_0)$; continuity rules out a strict deficit at any boundary point. This holds for every $0<r<R$, so $u$ is constant on the entire disk.

The [Cauchy-Riemann equations](../../../../../../../cauchy-riemann-equations.md) then give both partial derivatives of $v=\Im f$ equal to zero there. Thus $f$ is constant on that disk. The [identity theorem for holomorphic functions](../../../../../../../identity-theorem.md) propagates this constant to the connected component of $z_0$ in $U$. Applying the same Brownian argument to $v$ proves the assertion for the imaginary part as well:

$$
\boxed{\text{A local maximum of }\Re f\text{ or }\Im f\text{ forces }f\text{ to be constant on that component of }U.}
$$

If $U$ is connected, this is constancy on all of $U$. For a disconnected open set the printed global wording needs this qualification: a function taking different constants on two disjoint disks is holomorphic and has local maxima on each disk while not being globally constant.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 28](../../../../paper-28-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
