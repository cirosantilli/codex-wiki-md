<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the [optical trap](../../../../../optical-tweezers.md), use the trap-frame coordinate $y=x-v_Tt$ and the force-induced speed $u(y)=F(y)/\zeta$. Then $\dot y=u(y)-v_T$. The particle first enters the support at $y=X_R$ and exits at $y=-X_L$. Thus the actual support width is $w=X_R+X_L$. The printed difference $X_R-X_L$ is inconsistent with those endpoints and would give zero width for the symmetric example; below use the geometrically correct $w=2X_0$.

A [sufficient escape condition for a translating trap](../../../../../sufficient-escape-condition-for-a-translating-trap.md) is

$$
\boxed{v_T>\sup_y u(y).}
$$

For a bounded continuous force this makes the relative velocity strictly negative and bounded away from zero, ensuring finite passage. For an ordinary smooth well, a root of $u(y)=v_T$ met from the incident side instead prevents passage: the trajectory approaches a trap-frame equilibrium. At the limiting maximum-speed equality, the passage time can diverge. Under the strict condition, [passage through a translating optical trap](../../../../../passage-through-a-translating-optical-trap.md) gives

$$
\boxed{\Delta t=\int_{-X_L}^{X_R}\frac{dy}{v_T-u(y)},\qquad
\Delta x=\int_{-X_L}^{X_R}\frac{u(y)}{v_T-u(y)}\,dy
=v_T\Delta t-w.}
$$

The time is the support-crossing time; gaps where the force vanishes inside that interval are included.

There is an essential qualification to the direction claim. [Compact support](../../../../../compact-support.md) of $F$ alone does not imply positive displacement. For example, $F=-F_0<0$ throughout the support gives $\Delta x=-w(F_0/\zeta)/(v_T+F_0/\zeta)<0$ and satisfies the strict passing condition. A smooth negative bump is also a counterexample. The intended [optical trap](../../../../../optical-tweezers.md) is a localized conservative well with $F=-U'$ and equal outside potential values. This additional assumption gives $\int u\,dy=0$. Now

$$
\frac{u}{v_T-u}=\frac{u}{v_T}+\frac{u^2}{v_T(v_T-u)},\qquad
\boxed{\Delta x=\int_{-X_L}^{X_R}\frac{u(y)^2}{v_T[v_T-u(y)]}\,dy\geq0.}
$$

It is strictly positive for a nonzero force on a set of positive measure. This is [forward displacement from a translating localized potential](../../../../../forward-displacement-from-a-translating-localized-potential.md). During motion in the trap direction, the relative passage is slower, so the positive-force side acts longer; opposite motion speeds passage through the negative-force side. A complementary energy argument makes the sign transparent:

$$
\frac{dU}{dt}=-\zeta\dot x^2+v_T\zeta\dot x,
\qquad U_{\rm exit}=U_{\rm entry}
\quad\Longrightarrow\quad
v_T\Delta x=\int\dot x^2dt\geq0.
$$

The moving well must supply the viscous energy loss.

For the [high-speed passage expansion of a localized trap](../../../../../high-speed-passage-expansion-of-a-localized-trap.md), require $\|u\|_\infty/v_T\ll1$. Expanding the denominator uniformly gives

$$
\Delta x=\frac1{v_T}\int u\,dy+\frac1{v_T^2}\int u^2\,dy+O(v_T^{-3}).
$$

Therefore the localized conservative well has

$$
\boxed{\Delta x\sim\frac1{\zeta^2v_T^2}\int F(y)^2dy,\qquad
\Delta t=\frac{w}{v_T}+\frac1{\zeta^2v_T^3}\int F(y)^2dy+O(v_T^{-4}).}
$$

For a symmetric well the force is odd, the cubic moment vanishes, and the displacement remainder improves to $O(v_T^{-4})$. For an arbitrary compact force without equal outside potential levels, its signed area instead gives the leading $v_T^{-1}$ displacement.

For circular motion, let $C=2\pi R$ and use the local arclength model, with nonoverlapping support $w<C$. In each encounter the relative position traverses $w$, while the particle advances $\Delta x$. Outside the support the particle is stationary and the trap must traverse the remaining relative arclength $C-w$. Hence the time between kicks and the [repeated kicks from a circular optical trap](../../../../../repeated-kicks-from-a-circular-optical-trap.md) response are

$$
T_{\rm kick}=\Delta t+\frac{C-w}{v_T},\qquad
\boxed{f_p=\frac{\Delta x}{C[\Delta t+(C-w)/v_T]}
=f_T\frac{\Delta x}{C-w+v_T\Delta t}
=f_T\frac{\Delta x}{C+\Delta x}.}
$$

The last equality uses the single-passage identity. Equivalently, kicks arrive at the relative lap frequency $f_T-f_p$.

The precise small-correction condition for the [large-speed approximation for circular-trap kicks](../../../../../large-speed-approximation-for-circular-trap-kicks.md) is $\Delta x/C\ll1$. A sufficient high-speed regime for a localized well is $v_T\gg\|F\|_\infty/\zeta$, with $w<C$ fixed: writing $\epsilon=\|u\|_\infty/v_T<1$, the positive-displacement integral bounds $\Delta x/C\leq(w/C)\epsilon^2/(1-\epsilon)$. Thus

$$
\boxed{f_p\simeq\frac{\Delta x}{2\pi R}f_T.}
$$

The locally straight force profile on a real circular track also presumes a trap width small relative to the radius; $R\gg a$ supplies the particle-size part of that approximation.

For the [triangular optical-trap response](../../../../../triangular-optical-trap-response.md), put $v_c=F/\zeta=Cf_c$, $\beta=v_T/v_c$ and $\alpha=w/C=X_0/(\pi R)$. In the passing regime $\beta>1$, the two constant-force halves give

$$
\Delta t=\frac{X_0}{v_T+v_c}+\frac{X_0}{v_T-v_c}
=\frac{wv_T}{v_T^2-v_c^2},\qquad
\Delta x=\frac{wv_c^2}{v_T^2-v_c^2}=\frac{w}{\beta^2-1}.
$$

Substitution into the circular formula yields

$$
\boxed{\frac{f_p}{f_c}=\frac{\alpha\beta}{\beta^2-1+\alpha}\quad(\beta>1).}
$$

For $0<\beta\leq1$, the particle remains locked to the trap and $f_p/f_c=\beta$. At the ideal triangular cusp this is understood as sticking, or as the limit of a rounded well; it is not a finite passing kick. The passing branch tends continuously to one at $\beta\downarrow1$, while at large $\beta$ it behaves as $\alpha/\beta$. The zero-speed limiting response is zero. These branches apply to separated kicks, $0<\alpha<1$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
