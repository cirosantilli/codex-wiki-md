<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $G=g(\rho_p-\rho_0)/\rho_0$ and $b=G\phi>0$, the [reduced gravity](../../../../../../reduced-gravity-split.md). Use the [Boussinesq approximation](../../../../../../boussinesq-approximation.md), [hydrostatic pressure](../../../../../../hydrostatic-pressure.md), uniform vertical [velocity](../../../../../../velocity.md) and concentration profiles, negligible [fluid entrainment](../../../../../../fluid-entrainment.md) and drag, and a flat bed. Integrating [volume conservation](../../../../../../volume-conservation.md), [momentum conservation](../../../../../../momentum-conservation.md) and the particle budget over the layer gives

$$
h_t+(hu)_x=0,\qquad (hu)_t+\left(hu^2+\frac12bh^2\right)_x=0,\qquad (h\phi)_t+(hu\phi)_x=-V_s\phi.
$$

The [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) resultant is $\rho_0bh^2/2$; the last right-hand side is the [deposition flux](../../../../../../particle-deposition-flux.md). With $D=\partial_t+u\partial_x$, these are

$$
Dh=-hu_x,\qquad Du=-bh_x-\frac h2b_x,\qquad Db=-\frac{V_sb}{h}.
$$

The quasilinear coefficient [matrix](../../../../../../matrix.md) in variables $(h,u,b)$ is

$$
\begin{pmatrix}u&h&0\\b&u&h/2\\0&0&u\end{pmatrix}.
$$

Its [eigenvalues](../../../../../../eigenvalue.md) are $u,u\pm c$, where $c=\sqrt{bh}$. Therefore the [characteristic curves](../../../../../../characteristic-curve.md) and their compatibility [ordinary differential equations](../../../../../../ordinary-differential-equation.md) are

$$
\boxed{\frac{dx_0}{dt}=u,\quad \frac{db}{dt}=-\frac{V_sb}{h};\qquad \frac{dx_\pm}{dt}=u\pm c,\quad du\pm\frac ch\,dh\pm\frac h{2c}\,db=\mp\frac{V_sc}{2h}\,dt}.
$$

For the last equation the [left eigenvectors](../../../../../../left-eigenvector.md) are $(\pm c/h,1,\pm h/(2c))$, and multiplying the quasilinear equations by them gives the displayed source terms. This is the [sedimenting rectangular-channel characteristic compatibility](../../../../../../sedimenting-rectangular-channel-characteristic-compatibility.md) relation; it supplies one differential relation on each wave family, rather than three independently closed scalar equations there. The contact [eigenvector](../../../../../../eigenvector.md) has $du=0$ and $d(bh^2)=0$. For reference, an equivalent form is

$$
D_\pm(u\pm2c)=\frac h2b_x\mp\frac{V_sc}{h},\qquad D_\pm=\partial_t+(u\pm c)\partial_x.
$$

Only for constant $b$ without settling do $u\pm2c$ become genuine [Riemann invariants](../../../../../../riemann-invariant.md). With settling, the spatial buoyancy gradient cannot be silently omitted.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
