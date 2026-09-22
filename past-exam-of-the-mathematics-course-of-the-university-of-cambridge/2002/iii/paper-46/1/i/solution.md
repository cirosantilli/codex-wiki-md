<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the [gravitational potential](../../../../../../newtonian-potential-of-a-point-mass.md) with [spherical symmetry](../../../../../../spherical-symmetry.md) as $\Phi(r)$ and let $\mathbf n$ be the unit [vector](../../../../../../vector.md) normal to a [circular orbit](../../../../../../circular-orbit.md), oriented in the direction of its [angular velocity](../../../../../../angular-velocity.md). Put $\boldsymbol\Omega=\Omega\mathbf n$ and denote the [specific angular momentum](../../../../../../specific-angular-momentum.md) by $\mathbf h=h\mathbf n$. Circular force balance and the [specific orbital energy](../../../../../../specific-orbital-energy.md) give

$$
\Phi'(r)=r\Omega^2,\qquad h=r^2\Omega,\qquad \varepsilon=\Phi(r)+\frac12r^2\Omega^2.
$$

Differentiating along the family of [circular orbits](../../../../../../circular-orbit.md),

$$
\frac{d\varepsilon}{dr}=2r\Omega^2+r^2\Omega\Omega'=\Omega\frac{dh}{dr}.
$$

A change in orbital orientation contributes $h\,d\mathbf n$ to $d\mathbf h$, but $\mathbf n\cdot d\mathbf n=0$. Consequently

$$
\boxed{d\varepsilon=\Omega\,dh=\boldsymbol\Omega\cdot d\mathbf h.}
$$

This [circular-orbit energy gradient](../../../../../../circular-orbit-energy-gradient.md) accounts for radial and inclination changes together; [spherical symmetry](../../../../../../spherical-symmetry.md) makes the orbital [energy](../../../../../../energy.md) independent of the plane.

For either variable-mass particle, $\mathbf H=M\mathbf h$ and $E=M\varepsilon$. Thus $d\mathbf H=M\,d\mathbf h+\mathbf h\,dM$, so

$$
dE=\varepsilon\,dM+M\boldsymbol\Omega\cdot d\mathbf h=(\varepsilon-\Omega h)dM+\boldsymbol\Omega\cdot d\mathbf H.
$$

[Conservation of mass](../../../../../../mass-conservation.md) and [conservation of angular momentum](../../../../../../conservation-of-angular-momentum.md) impose $dM_2=-dM_1$, $d\mathbf H_2=-d\mathbf H_1$. Adding the two particle contributions proves

$$
\boxed{dE=\{(\varepsilon_1-\Omega_1h_1)-(\varepsilon_2-\Omega_2h_2)\}\,dM_1+(\boldsymbol\Omega_1-\boldsymbol\Omega_2)\cdot d\mathbf H_1.}
$$

To interpret the signs, label the inner orbit 1 and the outer orbit 2. For $f(r)=\varepsilon-\Omega h$ the first identity gives $f'=-h\Omega'$. The assumed outward decrease of [angular velocity](../../../../../../angular-velocity.md) therefore makes $f_1<f_2$, so the mass-exchange part lowers the [energy](../../../../../../energy.md) when $dM_1>0$: [mass](../../../../../../mass.md) is transferred inward. In a coplanar, co-rotating pair, $\Omega_1>\Omega_2$ and an outward [angular momentum](../../../../../../angular-momentum.md) transfer has $d\mathbf H_1=-dH\mathbf n$ with $dH>0$. Its contribution is $-(\Omega_1-\Omega_2)dH<0$.

The [vector](../../../../../../vector.md) difference also identifies the inclination-reducing exchange. For a fixed small magnitude of admissible [angular momentum](../../../../../../angular-momentum.md) exchange, its [energy](../../../../../../energy.md) contribution is most negative when

$$
d\mathbf H_1=-s(\boldsymbol\Omega_1-\boldsymbol\Omega_2),\qquad s>0,
$$

by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). This gives $dE_{\rm angular}=-s|\boldsymbol\Omega_1-\boldsymbol\Omega_2|^2$. Let $q=\mathbf n_1\cdot\mathbf n_2=\cos\iota$ and $H_i=|\mathbf H_i|$, taking fixed particle masses for this exchange. Projecting $d\mathbf H_i$ perpendicular to its own direction gives

$$
d\mathbf n_1=\frac{s\Omega_2}{H_1}(\mathbf n_2-q\mathbf n_1),\qquad d\mathbf n_2=\frac{s\Omega_1}{H_2}(\mathbf n_1-q\mathbf n_2).
$$

Therefore

$$
dq=s(1-q^2)\left(\frac{\Omega_2}{H_1}+\frac{\Omega_1}{H_2}\right)>0\qquad(0<\iota<\pi).
$$

The downhill exchange reduces the relative [orbital inclination](../../../../../../orbital-inclination.md). Its inner [angular momentum](../../../../../../angular-momentum.md) component is $\mathbf n_1\cdot d\mathbf H_1=-s(\Omega_1-\Omega_2q)<0$; in the aligned limit the outer orbit receives that [angular momentum](../../../../../../angular-momentum.md) directly. For strongly inclined orbits, part of the exchange instead cancels differently directed angular momenta as the planes align. Together these gradients explain the tendencies toward inward [mass](../../../../../../mass.md) transfer, outward [angular momentum](../../../../../../angular-momentum.md) transport and coplanarity.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
