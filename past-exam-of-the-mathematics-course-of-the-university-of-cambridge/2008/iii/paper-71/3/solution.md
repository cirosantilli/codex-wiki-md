<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Each annulus has a [torque](../../../../../torque.md) proportional to $\mathbf J_h\times\delta\mathbf J_d$, so its scalar product with $\mathbf J_h$ is zero. Summing over annuli preserves this property even when the proportionality coefficient varies with radius. Therefore $\boxed{\mathbf T\cdot\mathbf J_h=0}$ for the total [torque](../../../../../torque.md) due to [Lense-Thirring precession](../../../../../lense-thirring-precession.md).

The [torque](../../../../../torque.md) specified is the [torque](../../../../../torque.md) on the disk. Assuming a closed disk-plus-hole angular-momentum budget with no external [torque](../../../../../torque.md), its reaction on the [black hole](../../../../../black-hole.md) has the opposite sign:

$$
\boxed{\dot{\mathbf J}_h=-\mathbf T
=-K_1\mathbf J_h\times\mathbf J_d
-K_2\mathbf J_h\times(\mathbf J_h\times\mathbf J_d),\qquad
\dot{\mathbf J}_d=\mathbf T.}
$$

Thus $\dot{\mathbf J}_t=0$. The $K_1$ term describes [precession](../../../../../precession.md), because it is perpendicular to both spins. Since $\mathbf J_h\times\mathbf J_d=\mathbf J_h\times\mathbf J_t$, the hole precesses about the fixed total vector. The $K_2$ term changes the spin directions dissipatively. Writing $\mathbf J_{d,\perp}$ for the disk component perpendicular to the hole, the [vector triple product identity](../../../../../vector-triple-product.md) gives

$$
\mathbf J_h\times(\mathbf J_h\times\mathbf J_d)=-J_h^2\mathbf J_{d,\perp}.
$$

A positive $K_2$ removes this component from the disk and transfers it into the hole's changing direction. This is [black-hole and disk alignment under internal torque](../../../../../black-hole-and-disk-alignment-under-internal-torque.md).

Since $\mathbf T$ is perpendicular to $\mathbf J_h$,

$$
\frac d{dt}J_h^2=2\mathbf J_h\cdot\dot{\mathbf J}_h=-2\mathbf J_h\cdot\mathbf T=0.
$$

Hence $\boxed{J_h\text{ is constant}}$, even if the [torque](../../../../../torque.md) coefficients vary in time.

Now differentiate the scalar product with the conserved total vector. The [precession](../../../../../precession.md) term contributes zero, and the [vector triple product identity](../../../../../vector-triple-product.md) gives

$$
\begin{aligned}
\frac d{dt}(\mathbf J_h\cdot\mathbf J_t)
&=-\mathbf T\cdot(\mathbf J_h+\mathbf J_d)=-\mathbf T\cdot\mathbf J_d\\
&=K_2\left[J_h^2J_d^2-(\mathbf J_h\cdot\mathbf J_d)^2\right]\\
&=\boxed{K_2|\mathbf J_h\times\mathbf J_d|^2=A.}
\end{aligned}
$$

Also $\mathbf J_h\cdot\mathbf J_t=J_h^2+\mathbf J_h\cdot\mathbf J_d$, so constancy of $J_h$ gives

$$
\boxed{\frac d{dt}(\mathbf J_h\cdot\mathbf J_t)
=\frac d{dt}(\mathbf J_h\cdot\mathbf J_d).}
$$

Finally, $J_t^2=J_h^2+J_d^2+2\mathbf J_h\cdot\mathbf J_d$ is constant. Differentiating proves

$$
\boxed{\frac d{dt}J_d^2=-2A.}
$$

Thus the disk's spin magnitude decreases while the hole's magnitude is fixed; their vector sum remains fixed as well.

For the alignment conclusion, assume $J_h,J_t>0$ and let $c=\cos\theta=\mathbf J_h\cdot\mathbf J_t/(J_hJ_t)$. Since $\mathbf J_h\times\mathbf J_d=\mathbf J_h\times\mathbf J_t$,

$$
\boxed{\dot c=K_2J_hJ_t(1-c^2).}
$$

For a noncollinear initial state, $|c(0)|<1$, this integrates exactly to

$$
\operatorname{artanh}c(t)=\operatorname{artanh}c(0)+J_hJ_t\int_0^tK_2(s)\,ds.
$$

Consequently a fixed positive $K_2$, or more generally a positive coefficient of divergent integrated strength, gives $c(t)\to1$. In this persistent dissipative evolution, $\boxed{\mathbf J_h\to J_h\widehat{\mathbf J}_t}$: the hole aligns asymptotically with the total [angular momentum](../../../../../angular-momentum.md). The exactly antiparallel configuration $c=-1$ is a stationary, nongeneric exception; when $J_t=0$ there is no total-vector direction to align with.

If the phrase $K_2>0$ allows arbitrary time dependence, positivity alone does not logically force complete eventual alignment. The [persistent-torque criterion for asymptotic spin alignment](../../../../../persistent-torque-criterion-for-asymptotic-spin-alignment.md) is the needed qualification. For example, take $J_h=J_t=1$, $K_1=0$, $K_2(t)=e^{-t}$ and $c(0)=0$. The same [torque](../../../../../torque.md) equations give $c(t)=\tanh(1-e^{-t})$, with limit $\tanh1<1$. The final configurations below use the intended persistent-[torque](../../../../../torque.md) regime, including constant positive $K_2$.

Once the hole has aligned, [conservation of angular momentum](../../../../../conservation-of-angular-momentum.md) fixes the disk without any additional [torque](../../../../../torque.md) calculation:

$$
\boxed{\mathbf J_{h,f}=J_h\widehat{\mathbf J}_t,\qquad
\mathbf J_{d,f}=(J_t-J_h)\widehat{\mathbf J}_t.}
$$

The disk and hole therefore finish parallel only if $J_t>J_h$. If $J_t<J_h$, they finish antiparallel: this is [counteralignment of a black hole and accretion disk](../../../../../counteralignment-of-a-black-hole-and-accretion-disk.md). In terms of the initial disk-hole angle $\theta_0$, squaring $J_t$ shows that counteralignment occurs when

$$
\boxed{\cos\theta_0<-\frac{J_{d,0}}{2J_h}.}
$$

If $J_t=J_h$, the final disk [angular momentum](../../../../../angular-momentum.md) vanishes and has no spin direction. Thus alignment of the hole with the total vector does not imply alignment of both component spins.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
