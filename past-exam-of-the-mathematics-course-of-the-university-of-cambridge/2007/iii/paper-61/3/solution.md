<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\gamma_{\alpha\beta}=\delta_{\alpha\beta}$ be the positive Euclidean spatial background metric. Write a tensor-sector [metric perturbation](../../../../../linearized-gravity.md) as $h_{00}=h_{0\alpha}=0$, $h_{\alpha\beta}=-2E_{\alpha\beta}$, with $\gamma^{\alpha\beta}E_{\alpha\beta}=0$ and $\partial^\alpha E_{\alpha\beta}=0$. Spatial indices here are raised with $\gamma$, and $\Box=\partial_t^2-\Delta$.

Substitute the [linearized Levi-Civita connection](../../../../../linearized-levi-civita-connection.md) into the cover's curvature definition. To first order,

$$
\delta C_{ab}=\frac12\left(\Box h_{ab}+\partial_a\partial_bh-\partial_a\partial^ch_{bc}-\partial_b\partial^ch_{ac}\right),\qquad
\delta C=\Box h-\partial_a\partial_bh^{ab}.
$$

In the transverse-traceless tensor sector $h=0$ and $\partial^ch_{ac}=0$, so $\delta C=0$ and

$$
\delta G_{\alpha\beta}=\tfrac12\Box h_{\alpha\beta}=-\Box E_{\alpha\beta}.
$$

The tensor part of the [Linearized Einstein equations](../../../../../linearized-einstein-equations.md) therefore gives

$$
\boxed{\ddot E^{\alpha\beta}-\Delta E^{\alpha\beta}=8\pi G\,\delta\widehat T^{\alpha\beta}.}
$$

In a calculation strictly confined to the tensor sector, the source on this equation means its tensor projection; it is already trace-free there.

For a generic compact source, **trace-free is not the same as transverse-traceless**. For example, the static compactly supported spatial stress $T^{ij}=\partial^i\partial^j\chi-\gamma^{ij}\Delta\chi$, with smooth compactly supported $\chi$, is divergence-free, but its trace-free part has divergence $2\partial^j\Delta\chi/3$, generally nonzero. There is a precise way to reproduce the unprojected trace-free formula used in the question while retaining this distinction. In [Lorenz gauge in linearized gravity](../../../../../lorenz-gauge-in-linearized-gravity.md), the [trace-reversed metric perturbation](../../../../../trace-reversed-metric-perturbation.md) $\bar h_{ab}=h_{ab}-\eta_{ab}h/2$ obeys

$$
\partial^a\bar h_{ab}=0,\qquad \delta G_{ab}=\tfrac12\Box\bar h_{ab},\qquad
\Box\bar h_{ab}=-16\pi G\,\delta T_{ab}.
$$

Define its spatial trace-free half-strain by

$$
E_{\alpha\beta}=-\frac12\left(\bar h_{\alpha\beta}-\frac13\gamma_{\alpha\beta}\gamma^{\mu\nu}\bar h_{\mu\nu}\right).
$$

Then its wave equation has exactly the displayed trace-free source $\delta\widehat T^{\alpha\beta}=\delta T^{\alpha\beta}-\gamma^{\alpha\beta}\delta T^\mu{}_{\mu,\mathrm{spatial}}/3$. The physical tensor radiation is obtained afterwards with the [transverse-traceless projector](../../../../../transverse-traceless-projector.md). Without that projection, this $E$ is a Lorenz-gauge trace-free coefficient, not necessarily a transverse tensor mode. At leading far-zone order, the same directional projector is applied to both sides of the quadrupole field formula below.

The flat [contracted Bianchi identity](../../../../../contracted-bianchi-identity.md) implies [stress-energy conservation](../../../../../stress-energy-conservation.md), $\partial_b\delta T^{ab}=0$. Let

$$
I^{\alpha\beta}(t)=\int\delta T^{00}(t,\mathbf x)x^\alpha x^\beta\,d^3x.
$$

Compact support removes boundary terms. Differentiate and integrate by parts once:

$$
\begin{aligned}
\dot I^{\alpha\beta}
&=-\int\partial_\mu\delta T^{0\mu}\,x^\alpha x^\beta\,d^3x\\
&=\int\left(\delta T^{0\alpha}x^\beta+\delta T^{0\beta}x^\alpha\right)d^3x.
\end{aligned}
$$

A second time derivative, another integration by parts and symmetry of the [stress-energy tensor](../../../../../stress-energy-tensor.md) give

$$
\ddot I^{\alpha\beta}
=-\int\left(\partial_\mu\delta T^{\alpha\mu}x^\beta+\partial_\mu\delta T^{\beta\mu}x^\alpha\right)d^3x
=2\int\delta T^{\alpha\beta}\,d^3x.
$$

Take the spatial trace-free part. The [mass quadrupole moment](../../../../../mass-quadrupole-moment.md) satisfies the [stress-energy quadrupole identity](../../../../../stress-energy-quadrupole-identity.md)

$$
Q^{\alpha\beta}=I^{\alpha\beta}-\frac13\gamma^{\alpha\beta}\gamma_{\mu\nu}I^{\mu\nu},\qquad
\boxed{\ddot Q^{\alpha\beta}=2\int\delta\widehat T^{\alpha\beta}\,d^3x.}
$$

Inserting this into the assumed leading [retarded quadrupole field](../../../../../retarded-quadrupole-field.md) gives

$$
\boxed{E^{\alpha\beta}(t,\mathbf x)=\frac{G}{r}\ddot Q^{\alpha\beta}(t-r).}
$$

This is the requested spatial half-strain convention; the measured transverse-traceless strain is $H^{\mathrm{TT}}_{\alpha\beta}=2E^{\mathrm{TT}}_{\alpha\beta}$. The formula selects the retarded source field and does not include an independently added homogeneous [gravitational wave](../../../../../gravitational-wave.md). Dropping the source-dependent part of retardation also needs the [long-wavelength source approximation](../../../../../long-wavelength-source-approximation.md), besides $R/r\ll1$.

For a slowly moving weakly self-gravitating source, the [virial theorem](../../../../../virial-theorem.md) or the dynamical balance $v^2/R\sim GM/R^2$ gives $v^2\sim\epsilon=GM/R$. A varying nonspherical [mass quadrupole moment](../../../../../mass-quadrupole-moment.md) has characteristic size $MR^2$ and dynamical time $\tau\sim R/v$, so $\ddot Q\sim MR^2/\tau^2\sim Mv^2$. Consequently the [quadrupole strain scaling of a weak self-gravitating source](../../../../../quadrupole-strain-scaling-of-a-weak-self-gravitating-source.md) is

$$
\boxed{|E^{\alpha\beta}|=O\!\left(\frac{GM}{r}v^2\right)=O\!\left(\epsilon^2\frac{R}{r}\right).}
$$

This is a characteristic scale, not a nonzero lower bound: a stationary or exactly spherical source does not radiate. Slow motion gives $R/\tau\sim\sqrt\epsilon\ll1$, justifying the long-wavelength approximation; for a radiation-zone strain one also takes $r\gg\tau$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
