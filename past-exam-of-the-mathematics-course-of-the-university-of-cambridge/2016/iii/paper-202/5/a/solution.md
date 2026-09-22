<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Interpret $f$ as a [conformal bijection](../../../../../../biholomorphism.md) onto $D'$. If it is merely an injective map into a larger target, the correct exit domain is $f(D)$ instead. Let $\zeta$ be the exit time from $D$, write $f=u+iv$, and identify [planar Brownian motion](../../../../../../planar-brownian-motion.md) with $B^1+iB^2$. The [Cauchy-Riemann equations](../../../../../../cauchy-riemann-equations.md) give $u_x=v_y$, $u_y=-v_x$, and both $u,v$ are [harmonic functions](../../../../../../harmonic-function.md). The [Itô formula](../../../../../../ito-s-lemma.md), localized on compact subsets of $D$, yields

$$
du(B_t)=u_x(B_t)dB_t^1+u_y(B_t)dB_t^2,\qquad dv(B_t)=v_x(B_t)dB_t^1+v_y(B_t)dB_t^2.
$$

Thus both coordinates are [continuous local martingales](../../../../../../continuous-local-martingale.md), with

$$
[u(B)]_t=[v(B)]_t=A_t:=\int_0^{t}|f'(B_s)|^2ds,\qquad [u(B),v(B)]_t=\int_0^t(u_xv_x+u_yv_y)(B_s)ds=0\quad(t<\zeta).
$$

Since $f'$ never vanishes, $A$ is strictly increasing before $\zeta$. Let $\eta_s=\inf\{t:A_t>s\}$, defined for $s<A_{\zeta-}$. The [optional time-change theorem](../../../../../../optional-time-change-theorem.md) gives [continuous local martingale](../../../../../../continuous-local-martingale.md) coordinates for $\beta_s=f(B_{\eta_s})$, with bracket matrix $sI$. The [Lévy characterization of multidimensional Brownian motion](../../../../../../levy-characterization-of-multidimensional-brownian-motion.md) makes $\beta$ a standard [planar Brownian motion](../../../../../../planar-brownian-motion.md) started at $f(z)$, up to its lifetime. Therefore **[conformal invariance of planar Brownian motion](../../../../../../conformal-invariance-of-planar-brownian-motion.md) takes the form**

$$
\boxed{f(B_t)=\beta_{A_t},\qquad A_t=\int_0^t|f'(B_s)|^2ds,\quad t<\zeta.}
$$

To identify the lifetime, exhaust $D$ by relatively compact open sets $D_n$ with nested closures. The images $f(D_n)$ exhaust $D'$ because $f$ is a homeomorphism onto $D'$. Each stopped transformed path exits $f(D_n)$ at precisely the clock value of its exit from $D_n$. Increasing these exit times gives the exit lifetime of [Brownian motion](../../../../../../brownian-motion-split.md) from $D'$, including a possibly infinite lifetime. This identifies $A_{\zeta-}$ with that lifetime and needs no global extension of $f$ to the boundary.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
