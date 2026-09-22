<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [conformal invariance of planar Brownian motion](../../../../../../conformal-invariance-of-planar-brownian-motion.md) is a time-change statement. If $\phi:D\to D'$ is a conformal bijection of planar domains and $B$ is [planar Brownian motion](../../../../../../planar-brownian-motion.md) started in $D$, let $\tau_D$ be its exit time and define

$$
A_t=\int_0^{t\wedge\tau_D}|\phi'(B_s)|^2\,ds.
$$

Before exit this clock is strictly increasing. Its inverse $C_u$ makes $\phi(B_{C_u})$ a [planar Brownian motion](../../../../../../planar-brownian-motion.md) started at $\phi(B_0)$, up to its transformed lifetime $A_{\tau_D}$. The image of the stopped trajectory is therefore invariant in law after this change of time. A holomorphic map with nonzero derivative gives the corresponding local statement even without global injectivity.

Here is the proof. Write $\phi=u+iv$ and $B=(B^1,B^2)$. The real and imaginary parts are harmonic. The [Itô formula](../../../../../../ito-s-lemma.md) therefore gives the two [continuous local martingales](../../../../../../continuous-local-martingale.md)

$$
u(B_t)-u(B_0)=\int_0^t\nabla u(B_s)\cdot dB_s,
\qquad
v(B_t)-v(B_0)=\int_0^t\nabla v(B_s)\cdot dB_s,
$$

stopped on compact subsets of $D$. The [Cauchy-Riemann equations](../../../../../../cauchy-riemann-equations.md) imply

$$
|\nabla u|^2=|\nabla v|^2=|\phi'|^2,
\qquad\nabla u\cdot\nabla v=0.
$$

Thus both coordinate [quadratic variations](../../../../../../quadratic-variation.md) equal $A_t$ and their [quadratic covariation](../../../../../../quadratic-covariation.md) is zero. After inverse time change, the covariance matrix of the two [continuous local martingales](../../../../../../continuous-local-martingale.md) is $uI_2$. The multidimensional [Lévy characterization of multidimensional Brownian motion](../../../../../../levy-characterization-of-multidimensional-brownian-motion.md) states that a continuous vector [local martingale](../../../../../../local-martingale.md) starting at zero with this covariance matrix is standard vector [Brownian motion](../../../../../../brownian-motion-split.md). Apply it after subtracting $\phi(B_0)$, and exhaust $D$ by compact subsets. This proves the theorem, with killing at the transformed exit lifetime. The clock is the [conformal Brownian clock](../../../../../../conformal-brownian-clock.md); omitting it would generally give an incorrect speed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
