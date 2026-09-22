<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the state vector $q=(h,u,g')^T$, the primitive equations are $q_t+\mathsf A q_x=S$, with

$$
\mathsf A=\begin{pmatrix}u&h/2&0\\g'&u&h/3\\0&0&u\end{pmatrix},\qquad
S=\begin{pmatrix}w_e\\-2uw_e/h\\-2g'w_e/h\end{pmatrix}.
$$

The [characteristic polynomial](../../../../../../characteristic-polynomial.md) is

$$
\det(\mathsf A-\lambda I)=(u-\lambda)\left[(u-\lambda)^2-\frac{g'h}{2}\right].
$$

Consequently the three [characteristic speeds](../../../../../../characteristic-speed.md) are

$$
\boxed{\frac{dx}{dt}=u,\quad u+c,\quad u-c,\qquad c=\sqrt{\frac{g'h}{2}}.}
$$

For $h>0$ and $g'>0$, the [hyperbolic system](../../../../../../hyperbolic-system.md) has three distinct real [eigenvalues](../../../../../../eigenvalue.md). The long-wave speed relative to the current is $c$, while $u$ transports a [buoyancy](../../../../../../buoyancy.md)/contact disturbance.

A left [eigenvector](../../../../../../eigenvector.md) for the material characteristic is $(0,0,1)$, giving

$$
\boxed{\frac{dg'}{dt}=-\frac{2g'w_e}{h}\quad\text{along}\quad\frac{dx}{dt}=u.}
$$

For $u\pm c$, left [eigenvectors](../../../../../../eigenvector.md) can be chosen as

$$
\ell_\pm=\left(\pm\frac{2c}{h},1,\pm\frac{h}{3c}\right).
$$

Multiplying $q_t+\mathsf A q_x=S$ by these rows gives the [characteristic compatibility for an entraining triangular-channel current](../../../../../../characteristic-compatibility-for-an-entraining-triangular-channel-current.md). With all differentials evaluated along the indicated characteristic,

$$
\boxed{du\pm\frac{2c}{h}\,dh\pm\frac{h}{3c}\,dg'
=-\frac{2w_e}{h}\left(u\mp\frac c3\right)dt,
\qquad \frac{dx}{dt}=u\pm c.}
$$

The source follows directly from $\ell_\pm S=-2uw_e/h\pm2cw_e/h\mp2g'w_e/(3c)$ and $g'/c=2c/h$.

Since $4\,dc=(2c/h)dh+(h/c)dg'$, an equivalent form is

$$
d(u\pm4c)\mp\frac{4c}{3g'}\,dg'
=-\frac{2w_e}{h}\left(u\mp\frac c3\right)dt.
$$

Combining it with the material [buoyancy](../../../../../../buoyancy.md) equation also gives

$$
D_\pm(u\pm4c)=\frac{2h}{3}g'_x-\frac{2w_e}{h}(u\pm c),\qquad
D_\pm=\partial_t+(u\pm c)\partial_x.
$$

Only when [entrainment](../../../../../../fluid-entrainment.md) vanishes and $g'$ is spatially constant do $u\pm4c$ become constant [Riemann invariants](../../../../../../riemann-invariant.md) on these [characteristic curves](../../../../../../characteristic-curve.md). Dropping the [buoyancy](../../../../../../buoyancy.md) differential in the general problem would lose one of the required transport couplings. The characteristic formulas with $1/c$ apply to the nondegenerate region $g'h>0$; dry or neutrally buoyant limits require their conservative form instead.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 90](../../../paper-90-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
