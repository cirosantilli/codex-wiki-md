<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take $p$ as excess [pressure](../../../../../pressure.md) relative to the fluid far from the gap, and let $\dot h_0<0$ for approach. The lower surface of the sphere is $h_0+a-\sqrt{a^2-r^2}$ above the plane. In the dominant region $r=O(\sqrt{ah_0})\ll a$, this is the [parabolic lubrication gap](../../../../../parabolic-lubrication-gap.md)

$$
h(r,t)=h_0+\frac{r^2}{2a}+O(r^4/a^3).
$$

Its slope is $O(\sqrt{h_0/a})\ll1$, justifying [lubrication theory](../../../../../lubrication-theory.md). Both rigid surfaces have zero radial [velocity](../../../../../velocity.md), so the [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) and radial [Stokes equation](../../../../../stokes-equation.md) give the radial [volume flux](../../../../../volumetric-flow-rate.md) per unit circumference

$$
q=-\frac{h^3}{12\mu}p_r.
$$

Axisymmetric [conservation of mass](../../../../../mass-conservation.md) gives $h_t+r^{-1}(rq)_r=0$. Symmetry at $r=0$ therefore yields $q=-r\dot h_0/2$, hence $p_r=6\mu\dot h_0r/h^3$. Matching to $p\to0$ outside the pressure-bearing region gives

$$
\boxed{p=-3\mu a\dot h_0\left(h_0+\frac{r^2}{2a}\right)^{-2}.}
$$

Extending the parabolic profile to infinity in this integral is a leading-order matching device; the main [pressure](../../../../../pressure.md) and [force](../../../../../force.md) come from $r=O(\sqrt{ah_0})$.

The radial scale $\sqrt{a\widehat h}$ balances the two contributions to the gap. The time scale $\widehat h/\widehat v$ is the time for a typical gap change, and the [lubrication pressure](../../../../../lubrication-pressure.md) scale $\mu a\widehat v/\widehat h^2$ follows either from the formula above or from $p\sim\mu\widehat v\ell^2/\widehat h^3$ with $\ell^2=a\widehat h$. The elastic surface's upward displacement is $-\eta p$, so the actual gap is increased by $+\eta p$. Thus the dimensionless gap in [weakly compliant sphere-plane squeeze flow](../../../../../weakly-compliant-sphere-plane-squeeze-flow.md) is

$$
\mathcal H=H_0+\frac{R^2}{2}+\varepsilon P,\qquad
\boxed{\varepsilon=\frac{\eta\mu a\widehat v}{\widehat h^3}.}
$$

A dot now means differentiation with respect to $T$. The dimensionless [Reynolds lubrication equation](../../../../../reynolds-equation.md) is

$$
12\mathcal H_T=\frac1R\partial_R(R\mathcal H^3P_R).
$$

Even without fluid inertia, the elastic surface has a pressure-dependent normal [velocity](../../../../../velocity.md), so $\mathcal H_T$ includes $\varepsilon P_T$; omitting it would wrongly discard the acceleration term below.

Write $d=H_0+R^2/2$ and abbreviate $H=H_0$, $v=\dot H_0$, $b=\ddot H_0$ during the calculation. The rigid term is

$$
\boxed{P_0=-\frac{3v}{d^2}.}
$$

At first order the Reynolds equation gives

$$
\frac1R(Rd^3P_{1R})_R
=12P_{0T}-\frac1R(3Rd^2P_0P_{0R})_R
=-\frac{36b}{d^2}-\frac{144v^2}{d^3}+\frac{324Hv^2}{d^4}.
$$

Because $R\,dR=dd$, one integration gives

$$
Rd^3P_{1R}=2k(T)+\frac{36b}{d}+\frac{72v^2}{d^2}-\frac{108Hv^2}{d^3}.
$$

Set $\xi=R^2/(2H)$, so $d=H(1+\xi)$. Dividing and changing variables yields

$$
P_{1\xi}=\frac{k}{H^3\xi(1+\xi)^3}
+\frac{18b}{H^4\xi(1+\xi)^4}
-\frac{18v^2}{H^5\xi(1+\xi)^5}
+\frac{54v^2}{H^5(1+\xi)^6}.
$$

The first three terms are derivatives of $I_3,I_4,I_5$, respectively. Integrating from infinity to enforce $P_1\to0$ gives

$$
P_1=\frac{k}{H^3}I_3(\xi)+\frac{18b}{H^4}I_4(\xi)
-\frac{18v^2}{H^5}I_5(\xi)-\frac{54v^2}{5H^5}(1+\xi)^{-5}.
$$

The rational expansion of $I_n$ follows by differentiating $\log[\xi/(1+\xi)]+\sum_{j=1}^{n-1}[j(1+\xi)^j]^{-1}$, obtaining $1/[\xi(1+\xi)^n]$, and fixing its value to zero at infinity.

Near $\xi=0$ every $I_n$ has the same singular term $\log\xi$. Its coefficient must vanish to keep the [pressure](../../../../../pressure.md) regular, so

$$
\frac{k}{H^3}+\frac{18b}{H^4}-\frac{18v^2}{H^5}=0,
\qquad
\boxed{k=18\left(\frac{v^2}{H^2}-\frac bH\right).}
$$

Equivalently, the integrated radial flux above must vanish at $R=0$; otherwise $P_{1R}$ would have a $1/R$ singularity. Using $I_4=I_3+[3(1+\xi)^3]^{-1}$ and $I_5=I_4+[4(1+\xi)^4]^{-1}$ cancels all logarithms and gives the simplified regular expression

$$
\boxed{P_1=\frac{6\ddot H_0}{H_0^4}(1+\xi)^{-3}
-\frac{\dot H_0^2}{H_0^5}\left[6(1+\xi)^{-3}+\frac92(1+\xi)^{-4}+\frac{54}{5}(1+\xi)^{-5}\right].}
$$

The upward hydrodynamic [force](../../../../../force.md) has scale $\mu a^2\widehat v/\widehat h$. Its leading contribution is [pressure](../../../../../pressure.md) integrated over horizontal projected area; vertical shear [forces](../../../../../force.md) are smaller in the lubrication limit. Thus $F=2\pi\int_0^\infty(P_0+\varepsilon P_1+\cdots)R\,dR$. Use $R\,dR=H_0\,d\xi$ and $\int_0^\infty(1+\xi)^{-n}\,d\xi=1/(n-1)$. The two contributions are

$$
2\pi\int P_0R\,dR=-\frac{6\pi\dot H_0}{H_0},\qquad
2\pi\int P_1R\,dR=6\pi\left(\frac{\ddot H_0}{H_0^3}-\frac{12}{5}\frac{\dot H_0^2}{H_0^4}\right).
$$

Therefore

$$
\boxed{F=6\pi\left[-\frac{\dot H_0}{H_0}+\varepsilon\left(\frac{\ddot H_0}{H_0^3}-\frac{12}{5}\frac{\dot H_0^2}{H_0^4}\right)+\cdots\right].}
$$

For weight-controlled sedimentation, let the fixed effective load be $F=6\pi A$, $A>0$, and neglect particle inertia as well as fluid inertia. At leading order $\dot H_0=-AH_0$ and $\ddot H_0=A^2H_0$. The first-order bracket evaluated on this trajectory is $-(7/5)A^2/H_0^2$. Solving the [force](../../../../../force.md) balance perturbatively therefore gives

$$
\boxed{\dot H_0=-AH_0-\varepsilon\frac{7A^2}{5H_0}+O(\varepsilon^2).}
$$

Hence **weak compliance initially increases the sedimentation speed** in the regime where the perturbation is valid. The squeeze [pressure](../../../../../pressure.md) indents the coating away from the sphere, widens the flow passage and lowers resistance. This is a load-controlled conclusion on the slow sedimenting branch, not a claim about an arbitrary externally imposed acceleration at startup.

The [load-controlled breakdown of weak squeeze-flow compliance](../../../../../load-controlled-breakdown-of-weak-squeeze-flow-compliance.md) occurs when the relative correction $O(\varepsilon A/H_0^2)$ becomes order one:

$$
\boxed{H_0^*\sim\sqrt{\varepsilon A},\qquad H_0^*\sim\sqrt\varepsilon\ \hbox{for }A=O(1).}
$$

The central rigid [pressure](../../../../../pressure.md) has size $P_0(0)\sim A/H_0$, so the relative elastic gap change is also $\varepsilon P_0(0)/H_0\sim\varepsilon A/H_0^2$. Thus breakdown means that elastic deflection is comparable with the nominal undeformed gap. The regular expansion about a rigid plane then ceases to be uniform and the coupled elastic-lubrication problem must be retained. It does not by itself imply contact, fluid inertia or failure of the thin-gap geometry.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 66](../../paper-66-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
