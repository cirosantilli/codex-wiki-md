<h1 id="1/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Use an [asymptotic expansion](../../../../../asymptotic-expansion-split.md) at fixed $z$, evaluating the [boundary conditions](../../../../../boundary-condition.md) at the instantaneous $z=h(x,t)$. At leading order, the downslope equation gives $\hat u_{0,zz}=0$. The wall condition and the surface condition $\bar u_z(h)+\hat u_{0,z}(h)=0$ imply

$$
\boxed{\hat u_0=2(h-1)z,\qquad
u^{(0)}=\bar u+\hat u_0=2hz-z^2.}
$$

Here $u^{(0)}$ denotes the total leading [velocity](../../../../../velocity.md), to distinguish it from the dimensional scale $U_0$. The [continuity equation](../../../../../continuity-equation.md) and wall impermeability then give

$$
w^{(0)}=-z^2h_x.
$$

The transverse momentum equation gives $\hat p_{0,z}=0$. The [normal stress](../../../../../normal-stress.md) condition therefore yields

$$
\hat p_0=(h-1)\cot\alpha-\frac32S h_{xx},\qquad
p^{(0)}=(h-z)\cot\alpha-\frac32S h_{xx}.
$$

The leading [volume flux per unit width](../../../../../volume-flux-per-unit-width.md) is $q^{(0)}=\int_0^hu^{(0)}\,dz=2h^3/3$. Consequently [mass conservation](../../../../../mass-conservation.md) gives $h_t=-2h^2h_x+O(\varepsilon)$. This relation eliminates $h_t$ inside the first inertial correction:

$$
\begin{aligned}
u^{(0)}_t+u^{(0)}u^{(0)}_x+w^{(0)}u^{(0)}_z
&=2zh_t+(2hz-z^2)(2zh_x)-z^2h_x(2h-2z)\\
&=2hz(z-2h)h_x+O(\varepsilon).
\end{aligned}
$$

Set $G=2h_x\cot\alpha-3S h_{xxx}$. The $O(\varepsilon)$ downslope equation and [boundary conditions](../../../../../boundary-condition.md) are

$$
\hat u_{1,zz}=G+2\mathrm{Re}\,h h_x(z^2-2hz),\qquad
\hat u_1(0)=0,\quad \hat u_{1,z}(h)=0.
$$

Two [integrations](../../../../../integral-split.md) give

$$
\boxed{\hat u_1=G\left(\frac{z^2}{2}-hz\right)
+\mathrm{Re}\,h_x\left(\frac{hz^4}{6}-\frac{2h^2z^3}{3}+\frac{4h^4z}{3}\right).}
$$

The [pressure](../../../../../pressure-split.md) correction $\hat p_1$ is not needed for this calculation because its downslope [pressure gradient](../../../../../pressure-gradient.md) enters only at $O(\varepsilon^2)$.

Integrating the total [velocity](../../../../../velocity.md) across the film gives

$$
\begin{aligned}
q&=\int_0^h(\bar u+\hat u_0+\varepsilon\hat u_1)\,dz+O(\varepsilon^2)\\
&=\frac23h^3+\varepsilon\left[
-\frac{h^3}{3}G+\frac8{15}\mathrm{Re}\,h^6h_x\right]+O(\varepsilon^2).
\end{aligned}
$$

Indeed the three inertial [polynomial](../../../../../polynomial-split.md) terms integrate to $\mathrm{Re}\,h^6h_x(1/30-1/6+2/3)=8\mathrm{Re}\,h^6h_x/15$. Integrating the [continuity equation](../../../../../continuity-equation.md) and using the [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) gives $h_t+q_x=0$. Hence the [Benney equation](../../../../../benney-equation.md) is

$$
\boxed{h_t+2h^2h_x+\varepsilon\partial_x\left[
h^3\left(-\frac23h_x\cot\alpha+S h_{xxx}\right)
+\frac8{15}\mathrm{Re}\,h^6h_x\right]=0.}
$$

Normal [gravity](../../../../../gravity.md) smooths height variations on the upper side of the slope, while the inertial correction can amplify them. [Surface tension](../../../../../surface-tension-split.md) suppresses sufficiently short [wavelengths](../../../../../wavelength.md).

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../../split.md)
6. [Topics in fluid mechanics course of the University of Oxford](../../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
