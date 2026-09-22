<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $G=g\beta(T-T_0(z))$ for the plume [reduced gravity](../../../../../../reduced-gravity-split.md), and take $z$ upwards. For a symmetric [line plume](../../../../../../line-plume.md) define fluxes per unit source length,

$$
q=\int w\,dx,\qquad m=\int w^2\,dx,\qquad \mathcal B=\int wG\,dx.
$$

The integrals span the plume; its edges can move horizontally with $z$. The [fluid entrainment](../../../../../../fluid-entrainment.md) rate at one moving edge is the inward normal transport relative to that edge. For an edge $x=b(z)$ it is $E=wb'-u$; symmetry supplies equal transport through the other edge. The [Batchelor entrainment hypothesis](../../../../../../batchelor-entrainment-hypothesis.md) closes its mean value as $E=\alpha w_c$, where $w_c$ is a representative vertical [velocity](../../../../../../velocity.md) and $\alpha$ is the [entrainment coefficient](../../../../../../entrainment-coefficient.md). The integrated [volume conservation](../../../../../../volume-conservation.md) equation is therefore $q'=2\alpha w_c$.

Using [volume conservation](../../../../../../volume-conservation.md), the vertical acceleration equation has conservative form $\partial_x(uw)+\partial_z(w^2)=G$. Incoming ambient has zero vertical [momentum](../../../../../../momentum.md); the integrated [momentum conservation](../../../../../../momentum-conservation.md) equation is consequently $m'=\int G\,dx$. For the [temperature](../../../../../../temperature.md) anomaly, $T_0$ depends on height and

$$
\partial_x(uG)+\partial_z(wG)=-N^2w,\qquad N^2=g\beta\frac{dT_0}{dz}.
$$

Ambient fluid enters with $G=0$, giving the [buoyancy flux](../../../../../../buoyancy-flux.md) balance. The integral model is

$$
\boxed{q'=2\alpha w_c,\qquad m'=\int G\,dx,\qquad \mathcal B'=-N^2q.}
$$

Here $N$ is the [buoyancy frequency](../../../../../../buoyancy-frequency.md) when $N^2>0$; the same algebra permits unstable [temperature](../../../../../../temperature.md) gradients with $N^2<0$.

These are mean integral balances. The advective equations printed in the question omit explicit turbulent stresses and heat fluxes; a [turbulent plume](../../../../../../turbulent-plume-split.md) interpretation requires the usual entrainment closure for that unresolved transverse transport. Assuming vanishing edge stresses and heat fluxes, and negligible additional axial turbulent-flux contributions, gives the displayed bulk model. It would be inconsistent to treat a discontinuous top-hat profile as a smooth exact pointwise solution of the inviscid temperature-advection equation.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Section C](../../section-c.md)
4. [Paper 52](../../../paper-52-split.md)
5. [Iii](../../../split.md)
6. [2002](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
