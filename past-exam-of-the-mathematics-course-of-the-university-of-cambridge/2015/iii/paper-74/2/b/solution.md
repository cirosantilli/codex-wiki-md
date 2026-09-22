<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The channel is prismatic: its width depends on height, not on $x$. A layer of depth $h$ has cross-sectional area $A=\int_0^h\beta z\,dz=\beta h^2/2$. [Volume conservation](../../../../../../volume-conservation.md) gives $A_t+(Au)_x=0$. With $g'=G\phi$, the integrated excess [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) force is

$$
\frac1{\rho_0}\int_0^h p_{\rm excess}\,b(z)\,dz
=G\phi\int_0^h(h-z)\beta z\,dz=\frac{G\phi\beta h^3}{6}.
$$

Thus the streamwise [momentum](../../../../../../momentum.md) balance is $(Au)_t+(Au^2+G\phi\beta h^3/6)_x=0$. Under the specified vertical-settling approximation, the horizontal projection of the depositional boundary has width $\beta h$, so the particle balance is $(A\phi)_t+(Au\phi)_x=-\beta h\,w\phi$, where $w=w_0f(\phi)>0$ is the downward speed magnitude. The [prismatic triangular-channel shallow water equations](../../../../../../prismatic-triangular-channel-shallow-water-equations.md) are therefore

$$
\boxed{\begin{aligned}
h_t+uh_x+\frac h2u_x&=0,\\
u_t+uu_x+G\phi h_x+\frac{Gh}{3}\phi_x&=0,\\
\phi_t+u\phi_x&=-\frac{2w\phi}{h}.
\end{aligned}}
$$

The pressure coefficient $h/3$ is the section-weighted mean of $h-z$. The factor two in deposition comes from top width divided by area. There is no streamwise widening term, because $\beta$ is constant along the channel.

Define the positive [characteristic speed](../../../../../../characteristic-speed.md) scale $c=\sqrt{G\phi h/2}$. In variables $(u,\phi,c)$ the equations become

$$
\begin{aligned}
u_t+uu_x+4cc_x-\frac{4c^2}{3\phi}\phi_x&=0,\\
\phi_t+u\phi_x&=-\frac{2w\phi}{h},\\
c_t+uc_x+\frac c4u_x&=-\frac{wc}{h}.
\end{aligned}
$$

The coefficient matrix of this [hyperbolic system](../../../../../../hyperbolic-system.md) has [eigenvalues](../../../../../../eigenvalue.md) $u,u+c,u-c$. Hence **the three characteristic families are**

$$
\boxed{\frac{dx}{dt}=u,\qquad \frac{dx}{dt}=u\pm c.}
$$

Along $dx/dt=u$, the [concentration](../../../../../../concentration.md) equation is the ordinary differential equation $d\phi/dt=-2w\phi/h$. Along $dx/dt=u\pm c$, the left eigenvectors $(1,\mp4c/(3\phi),\pm4)$ give the [sedimenting triangular-channel characteristic compatibility](../../../../../../sedimenting-triangular-channel-characteristic-compatibility.md) equations

$$
\boxed{\frac{du}{dt}\pm4\frac{dc}{dt}\mp\frac{4c}{3\phi}\frac{d\phi}{dt}=\mp\frac{4wc}{3h}.}
$$

Here every derivative in a given equation follows that characteristic family, and $h=2c^2/(G\phi)$. These three compatibility equations form the characteristic description; they are not three independent closed equations for all fields on any one curve. In particular, $u\pm4c$ are not conserved [Riemann invariants](../../../../../../riemann-invariant.md) when the [concentration](../../../../../../concentration.md) varies: its differential and the deposition source must both be retained. The description assumes $h,\phi>0$; the dry or zero-buoyancy limit is degenerate.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
