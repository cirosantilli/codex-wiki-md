<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the convention that the coordinates of [planar Brownian motion](../../../../../../planar-brownian-motion.md) are independent standard real [Brownian motions](../../../../../../brownian-motion-split.md), so its [infinitesimal generator](../../../../../../infinitesimal-generator-stochastic-processes.md) is $\tfrac12\Delta$. Define the forward [conformal Brownian clock](../../../../../../conformal-brownian-clock.md)

$$
A(s)=\int_0^s|\phi'(B_r)|^2\,dr,\qquad
\widetilde T=A(T-),\qquad \tau=A^{-1}.
$$

Since a [conformal bijection](../../../../../../biholomorphism.md) has nonzero derivative, $A$ is a strictly increasing continuous map from $[0,T)$ onto $[0,\widetilde T)$. The time used inside the original path is its inverse:

$$
\boxed{\tau:[0,\widetilde T)\longrightarrow[0,T),\qquad
\widetilde B_t=\phi(B_{\tau(t)}).}
$$

Thus the interval direction for $\tau$ is the inverse-clock direction.

Write $\phi=u+iv$. The [Cauchy-Riemann equations](../../../../../../cauchy-riemann-equations.md) and the [Itô formula](../../../../../../ito-s-lemma.md) make $u(B_s),v(B_s)$ continuous [local martingales](../../../../../../local-martingale.md), with

$$
d[u(B)]_s=d[v(B)]_s=|\phi'(B_s)|^2ds,
\qquad d[u(B),v(B)]_s=0.
$$

Indeed both components are [harmonic functions](../../../../../../harmonic-function.md), and their gradients are orthogonal with the same squared norm. After the [time change of a continuous process](../../../../../../time-change-of-a-continuous-process.md) by $\tau$, their [quadratic variations](../../../../../../quadratic-variation.md) are $t$ and their [quadratic covariation](../../../../../../quadratic-covariation.md) is zero. The [Lévy characterization of multidimensional Brownian motion](../../../../../../levy-characterization-of-multidimensional-brownian-motion.md) therefore identifies $\widetilde B$ as [planar Brownian motion](../../../../../../planar-brownian-motion.md) started at $z'$, up to its lifetime.

It remains to identify that lifetime as the exit time, rather than merely produce a local Brownian path. Boundedness of $D$ gives $T<\infty$ [almost surely](../../../../../../almost-sure-convergence.md). For every compact subset $C\subset D'$, its inverse image under $\phi$ is compactly contained in $D$. As $s\uparrow T$, continuity gives $B_s\to B_T\notin D$, so $\phi(B_s)$ eventually leaves $C$. Consequently the transformed path leaves every compact subset of $D'$ at its lifetime. If $\widetilde T<\infty$, its Brownian extension has a finite limit, and that limit is outside $D'$; if $\widetilde T=\infty$, the path never exits. In both cases its maximal lifetime is precisely the exit time from $D'$.

**The killed paths, together with their lifetimes, have the same law**:

$$
\boxed{\bigl(\widetilde T,(\widetilde B_t)_{t<\widetilde T}\bigr)
\overset{d}=\bigl(T',(B'_t)_{t<T'}\bigr).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
