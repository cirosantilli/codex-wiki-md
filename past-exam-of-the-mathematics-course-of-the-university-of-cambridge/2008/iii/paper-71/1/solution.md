<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Assume an axisymmetric, geometrically [thin disc](../../../../../thin-disk.md) in a fixed [Keplerian rotation](../../../../../keplerian-disk.md) field, neglecting the disk's self-gravity. Write $v_R$ positive outwards and let

$$
\Omega(R)=\sqrt{\frac{GM}{R^3}},\qquad h(R)=R^2\Omega=\sqrt{GMR}.
$$

The ring supplies the local [specific angular momentum](../../../../../specific-angular-momentum.md). Its source per unit area is

$$
s(R,t)=\frac{\dot M(t)}{2\pi R_0}\delta(R-R_0),
$$

where the [Dirac delta function](../../../../../dirac-delta-function.md) is normalized so that $\int2\pi Rs\,dR=\dot M(t)$. Define the positive outward [viscous torque in an accretion disk](../../../../../viscous-torque-in-an-accretion-disk.md) by

$$
\mathcal G=-2\pi R^3\nu\Sigma\frac{d\Omega}{dR}=3\pi\nu\Sigma h.
$$

The height-integrated [conservation of mass](../../../../../mass-conservation.md) and [conservation of angular momentum](../../../../../conservation-of-angular-momentum.md) equations are

$$
\partial_t\Sigma+\frac1R\partial_R(R\Sigma v_R)=s,
$$



$$
\partial_t(\Sigma h)+\frac1R\partial_R(R\Sigma v_Rh)
=-\frac1{2\pi R}\partial_R\mathcal G+s h_0.
$$

Subtract $h$ times the mass equation. Since $h$ is time-independent, this gives

$$
\Sigma v_R h'=-\frac1{2\pi R}\mathcal G'+s(h_0-h).
$$

The last term is zero as a distribution, because the source is supported where $h=h_0$. Since $h'=h/(2R)$, substituting the [torque](../../../../../torque.md) gives

$$
v_R=-\frac3{\Sigma R^{1/2}}\partial_R(\nu\Sigma R^{1/2}).
$$

Inserting this into the mass equation proves the [Keplerian disk evolution with a ring source](../../../../../keplerian-disk-evolution-with-a-ring-source.md):

$$
\boxed{\partial_t\Sigma=\frac3R\partial_R\!\left[R^{1/2}\partial_R(\nu\Sigma R^{1/2})\right]
+\frac{\dot M(t)}{2\pi R_0}\delta(R-R_0).}
$$

The [viscosity](../../../../../dynamic-viscosity.md) may be a prescribed function or a function of the local disk state; the conservation derivation is the same.

To track signs in the steady problem, define the inward [mass flux](../../../../../mass-flux.md)

$$
F_M=-2\pi R\Sigma v_R=6\pi R^{1/2}\partial_R(\nu\Sigma R^{1/2}).
$$

Then $0=F_M'/(2\pi R)+s$. Away from the source $F_M$ is constant, with $F_M=\dot M_{\rm in}$ on the inner side and $F_M=-\dot M_{\rm out}$ on the outer side, where both loss rates are positive. Integrating through the source gives $F_M(R_0^+)-F_M(R_0^-)=-\dot M$. Therefore

$$
\boxed{\dot M=\dot M_{\rm in}+\dot M_{\rm out}.}
$$

The outward [angular momentum](../../../../../angular-momentum.md) flux is $F_J=\mathcal G-F_Mh$. The steady angular-momentum equation gives $F_J'=2\pi Rs h_0$. At the two [torque](../../../../../torque.md)-free boundaries its values are $F_J(R_{\rm in})=-\dot M_{\rm in}h_{\rm in}$ and $F_J(R_{\rm out})=\dot M_{\rm out}h_{\rm out}$. Integrating across the disk therefore yields

$$
\dot M h_0=\dot M_{\rm in}h_{\rm in}+\dot M_{\rm out}h_{\rm out}.
$$

Eliminate $\dot M_{\rm out}=\dot M-\dot M_{\rm in}$ and use $h\propto R^{1/2}$. The [two-boundary mass split of a ring-fed disk](../../../../../two-boundary-mass-split-of-a-ring-fed-disk.md) is

$$
\boxed{\frac{\dot M_{\rm in}}{\dot M}
=\frac{h_{\rm out}-h_0}{h_{\rm out}-h_{\rm in}}
=\frac{\sqrt{R_{\rm out}}-\sqrt{R_0}}{\sqrt{R_{\rm out}}-\sqrt{R_{\rm in}}}.}
$$

The complementary outward fraction is $(\sqrt{R_0}-\sqrt{R_{\rm in}})/(\sqrt{R_{\rm out}}-\sqrt{R_{\rm in}})$. Both fractions lie between zero and one for a source strictly between the boundaries.

As a local check, integrating the steady [mass flux](../../../../../mass-flux.md) from each zero-[torque](../../../../../torque.md) boundary gives

$$
\nu\Sigma\sqrt R=
\begin{cases}
\dfrac{\dot M_{\rm in}}{3\pi}(\sqrt R-\sqrt{R_{\rm in}}),&R_{\rm in}<R<R_0,\\
\dfrac{\dot M_{\rm out}}{3\pi}(\sqrt{R_{\rm out}}-\sqrt R),&R_0<R<R_{\rm out}.
\end{cases}
$$

Continuity of this quantity at $R_0$ gives the same split. The split depends on boundary and source angular momenta, rather than on the detailed [viscosity](../../../../../dynamic-viscosity.md) law.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
