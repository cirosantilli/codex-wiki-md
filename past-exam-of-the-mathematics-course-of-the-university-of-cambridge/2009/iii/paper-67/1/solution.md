<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use a planar flux function $F=B_0z+a$ and write

$$
\mathbf B=(F_z,0,-F_x).
$$

This automatically satisfies the [solenoidal magnetic-field constraint](../../../../../solenoidal-magnetic-field-constraint.md). There is a sign convention to settle: with the usual definition $\mathbf B=\nabla\times\mathbf A$, the [magnetic vector potential](../../../../../magnetic-vector-potential.md) is $\mathbf A=-F\widehat{\mathbf y}$. The positive sign printed for $A_y$ instead gives the opposite field, or corresponds to defining $\mathbf B=-\nabla\times\mathbf A$. We use the standard curl convention and the flux $F$ oriented along the prescribed positive $B_0$; the flux evolution and all transport identities below are unchanged by reversing the overall potential convention.

For planar [incompressible flow](../../../../../incompressible-flow.md), substitute this representation into the [resistive induction equation](../../../../../resistive-induction-equation.md). The two in-plane components imply

$$
F_t+\mathbf u\cdot\nabla F=\eta\nabla^2F+C(t).
$$

An additive time-dependent constant in $F$ leaves the field unchanged and removes $C(t)$. Since $\nabla^2(B_0z)=0$, this gives

$$
\boxed{a_t+\mathbf u\cdot\nabla a+B_0w=\eta\nabla^2a.}
$$

This is the scalar [advection-diffusion equation](../../../../../advection-diffusion-equation.md) underlying the [planar anti-dynamo theorem](../../../../../planar-anti-dynamo-theorem.md), with the imposed-field source retained.

Put $M(z)=\bar a(z)$, $a=M+a'$ and $F_c(z)=\overline{wa'}$. Stationarity of the horizontal averages, $\bar w=0$, and incompressibility give

$$
\partial_zF_c=\eta M''.
$$

Here the horizontal derivative of the advective flux has zero average. Integration gives $F_c=\eta M'+C$. Averaging once more, with $\langle M'\rangle=0$, identifies $C=\langle wa'\rangle$. Thus

$$
\boxed{\overline{wa'}=\eta\bar a_z+\langle wa'\rangle.}
$$

Decay or periodic averaging removes the endpoint contribution from the mean derivative. The periodic assumption used later replaces decay at vertical infinity; a nonzero periodic function cannot also decay there.

Subtract the averaged equation from the scalar equation and multiply by $a'$. The average of the time derivative is zero by stationarity; the advective term becomes a boundary flux and vanishes by incompressibility and the stated boundary averaging. Terms depending only on $z$ multiply $\overline{a'}=0$. [Integration by parts](../../../../../integration-by-parts.md) in the diffusion term therefore gives

$$
\boxed{\langle\overline{wa'}M'\rangle+B_0\langle wa'\rangle
=-\eta\langle|\nabla a'|^2\rangle.}
$$

Substituting $F_c=\eta M'+C$ and using $\langle M'\rangle=0$ yields the [Zeldovich planar flux balance](../../../../../zeldovich-planar-flux-balance.md)

$$
\boxed{B_0\langle wa'\rangle=-\eta\langle|\nabla a'|^2\rangle-\eta\langle(M')^2\rangle.}
$$

Both terms on the right are dissipative. In a nontrivial stationary forced problem this requires transport opposing the imposed flux gradient.

For finite-energy localized fields, enforcing decay at both vertical infinities literally gives $C=0$ from the mean-flux boundary values; the corresponding integral balance then forces both dissipation terms to vanish. The later nonzero-transport, periodic case therefore replaces that localized boundary setting rather than satisfying both simultaneously.

Now assume $B_0\ne0$ and a positive [turbulent magnetic diffusivity](../../../../../turbulent-magnetic-diffusivity.md) $\eta_1$. Define

$$
V=\langle(f-1)^2\rangle=\langle f^2\rangle-1,\qquad
r_t=\frac{\eta_1}{\eta},\qquad
G=\langle|\nabla a'|^2\rangle.
$$

Since $F_c=-\eta_1B_0f$ and $\langle f\rangle=1$, its spatial mean is $C=-\eta_1B_0$. Hence

$$
M'=-r_tB_0(f-1).
$$

The [Zeldovich planar flux balance](../../../../../zeldovich-planar-flux-balance.md) becomes

$$
\eta_1B_0^2=\eta G+\frac{\eta_1^2}{\eta}B_0^2V,
\qquad
G=r_tB_0^2(1-r_tV).
$$

Because $C\ne0$, the fluctuation cannot vanish, and a nontrivial fluctuation has $G>0$ under the stated boundary or zero-mean periodic conditions. Therefore

$$
\boxed{\frac{\eta}{\eta_1}>\langle f^2\rangle-1.}
$$

If $\eta_1\gg\eta$, then $\|f-1\|_{L^2}^2<\eta/\eta_1\ll1$: **the transport profile must be nearly constant in mean square.** This does not, without additional regularity, imply a uniform pointwise bound on narrow spikes.

For the final estimate use the supplied [Poincaré inequality](../../../../../poincare-inequality.md) in the periodic setting and the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md):

$$
\eta_1^2B_0^2=\langle wa'\rangle^2
\leq\langle w^2\rangle\langle a'^2\rangle
\leq\langle w^2\rangle\frac{d^2}{\pi^2}G.
$$

Insert the expression for $G$, cancel $B_0^2$, and multiply by $V$. Setting $y=r_tV\in[0,1)$ gives

$$
\eta_1^2V\leq\langle w^2\rangle\frac{d^2}{\pi^2}y(1-y)
\leq\langle w^2\rangle\frac{d^2}{4\pi^2}.
$$

Consequently the [variance bound for planar turbulent magnetic transport](../../../../../variance-bound-for-planar-turbulent-magnetic-transport.md) is

$$
\boxed{\eta_1^2[\langle f^2\rangle-1]\leq\langle w^2\rangle\frac{d^2}{4\pi^2}.}
$$

The factor $1/4$ comes from maximizing $y(1-y)$, so the weaker supplied Poincare constant already suffices. Under a zero vertical mean at each horizontal location, the usual period-$d$ Fourier bound is even stronger, with $4\pi^2/d^2$ in place of $\pi^2/d^2$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
