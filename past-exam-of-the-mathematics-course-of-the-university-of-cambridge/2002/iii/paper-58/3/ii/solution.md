<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use $\xi=x-\widehat X(T)$, $T=\varepsilon t$. At order $\varepsilon$, the moving-profile expansion gives

$$
-\widehat X_T A_0'(\xi)=\mathcal LR+\nu(\xi+\widehat X,T)A_0(\xi).
$$

The slow time derivative of $\varepsilon R$ is of order $\varepsilon^2$. Multiplication by $A_0'$ and integration eliminate $\mathcal LR$ by the [Fredholm solvability condition](../../../../../../fredholm-solvability-condition.md). Thus the leading velocity is

$$
\boxed{-\widehat X_T\int_{-\infty}^{\infty}(A_0')^2\,d\xi
=\int_{-\infty}^{\infty}\nu(\xi+\widehat X,T)A_0A_0'\,d\xi.}
$$

For $\nu(x,T)=K\delta(x+cT)$ the [Dirac delta](../../../../../../dirac-delta-function.md) samples $\xi=-\widehat X-cT$. From the first-order profile equation,

$$
\mathcal D=\int (A_0')^2\,d\xi
=\frac1{\sqrt3}\int_0^{\sqrt q}A(q-A^2)\,dA
=\frac{q^2}{4\sqrt3},\qquad
A_0A_0'=\frac1{\sqrt3}s(q-s).
$$

Consequently

$$
\boxed{\widehat X_T=-\frac{4Kq e^{\beta(\widehat X+cT)}}{(1+q e^{\beta(\widehat X+cT)})^2}
=-K\operatorname{sech}^2\!\left(\frac{\beta Z}{2}\right),\qquad
Z=\widehat X+cT+\frac{\log q}{\beta}.}
$$

The prefactor $q$ in the printed profile is important for the position shift in $Z$. This is a leading-order velocity in slow time; the physical velocity is $d\widehat X/dt=\varepsilon\widehat X_T+O(\varepsilon^2)$.

The relative position obeys the autonomous [moving-defect locking of a cubic-quintic front](../../../../../../moving-defect-locking-of-a-cubic-quintic-front.md) equation $Z_T=c-K\operatorname{sech}^2(\beta Z/2)$. For $K\ne0$, a finite constant-velocity front must have constant $Z$, and hence must travel with the defect at $\widehat X_T=-c$. Such locked fronts exist exactly when

$$
\boxed{0<\frac cK\le1.}
$$

For the strict inequality, their positions are

$$
Z_\pm=\pm\frac2\beta\operatorname{arcosh}\sqrt{\frac Kc},\qquad
\widehat X(T)=-cT-\frac{\log q}{\beta}+Z_\pm.
$$

Linearizing the relative-position equation gives $\eta_T=K\beta\operatorname{sech}^2(\beta Z_*/2)\tanh(\beta Z_*/2)\eta$. Therefore **the root with $KZ_*<0$ is stable and the other root unstable**. At $c=K$, they coalesce at $Z=0$ in a [saddle-node bifurcation](../../../../../../saddle-node-bifurcation.md). Since $Z_T=K\beta^2Z^2/4+O(Z^4)$ there, the double root attracts from only one side and is not two-sided asymptotically stable. Locking within its existence range still requires an initial relative position in the stable root's basin; beyond the unstable root the front escapes instead.

These positional stability conclusions also describe the leading weakly perturbed front. Indeed $v=A_0'>0$ has no zeros, and $\mathcal L=(\partial_\xi+v'/v)(\partial_\xi-v'/v)$ is nonpositive in the $L^2$ inner product. The limiting coefficients $f'(0)=-3\alpha^2/16$ and $f'(\sqrt q)=-3\alpha^2/4$ are negative. Thus the unperturbed shape modes are damped, with the neutral translation mode singled out by the [solvability condition](../../../../../../solvability-condition.md); the defect determines its stability at first order.

If $c\ne0$ and the locking inequality fails, $Z_T$ has no finite zero and has the sign of $c$. The separation grows without bound, the localized forcing of the front decays exponentially, and $\widehat X_T\to0$: the defect passes the front, which approaches a stationary position in laboratory coordinates. The same escaping behavior occurs outside the locking basin when roots exist. If $c=0$ and $K\ne0$, the stationary defect drives the front away from it with ever decreasing speed; $Z$ grows in magnitude logarithmically rather than tending to a finite locked position. Finally, when $K=0$, the front remains stationary for every $c$; when also $c=0$, every front position is a neutral equilibrium. These degenerate cases must not be included by dividing by $K$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
