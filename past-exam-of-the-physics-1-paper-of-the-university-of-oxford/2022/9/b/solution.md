<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take upward [velocity](../../../../velocity.md) as positive, and let $w>0$ be the rearward [rocket exhaust speed](../../../../rocket-exhaust-speed.md). During $dt$, the ejected parcel has [mass](../../../../mass.md) $-dm>0$ and laboratory [velocity](../../../../velocity.md) $v-w$ to first order. The [momentum](../../../../momentum-split.md) change of the rocket and this parcel equals the gravitational [impulse](../../../../impulse.md):

$$
(m+dm)(v+dv)+(-dm)(v-w)-mv=-mg\,dt.
$$

Discarding the second-order product $dm\,dv$ gives the vertical [rocket equation](../../../../rocket-equation.md)

$$
\boxed{m\frac{dv}{dt}=-w\frac{dm}{dt}-mg.}
$$

With $\dot m=-\alpha$ and $m=m_0-\alpha t$, integration for free flight starting from rest at $t=0$ gives

$$
\boxed{v(t)=w\ln\frac{m_0}{m_0-\alpha t}-gt,\qquad 0\le t\le T.}
$$

The logarithmic term is the ideal [Tsiolkovsky rocket equation](../../../../rocket-equation.md) contribution; $gt$ is the gravity loss. Immediate upward departure requires positive initial [acceleration](../../../../acceleration.md), or

$$
\boxed{\alpha w>m_0g,\qquad w_{\mathrm{threshold}}=\frac{m_0g}{\alpha}.}
$$

At exact equality the initial [acceleration](../../../../acceleration.md) is zero, but further burning reduces the weight and permits departure immediately thereafter. If departure is allowed to be delayed while fuel burns on the pad, the condition is instead $\alpha w>m(t)g$ at some time before burnout. With final [rocket dry mass](../../../../rocket-dry-mass.md) $m_f$, any powered departure before burnout requires $w>gm_f/\alpha$; the free-flight formula then starts at the actual departure time $t_\ell$ with $m(t_\ell)$, giving $v=w\ln[m(t_\ell)/m(t)]-g(t-t_\ell)$.

For the specified data, the initial [mass](../../../../mass.md) includes the payload. The [rocket fuel fraction](../../../../rocket-fuel-fraction.md) gives

$$
m_f=(1-f)m_0=2500\,\mathrm{kg},\qquad
T=\frac{fm_0}{\alpha}=15\,\mathrm s.
$$

The $100\,\mathrm{kg}$ payload is already part of the $2500\,\mathrm{kg}$ final [mass](../../../../mass.md); it is not the entire [rocket dry mass](../../../../rocket-dry-mass.md) and must not be added a second time. Here $m_0g/\alpha=196\,\mathrm{m/s}$, well below the stated [rocket exhaust speed](../../../../rocket-exhaust-speed.md), so departure is immediate. The burnout [speed](../../../../speed.md) is

$$
\boxed{v(T)=2500\ln4-9.8(15)\simeq3319\,\mathrm{m/s}.}
$$

This is the [speed](../../../../speed.md) at burnout. Subsequent motion under the assumed uniform [gravity](../../../../gravity.md) has $v(t)=v(T)-g(t-T)$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
