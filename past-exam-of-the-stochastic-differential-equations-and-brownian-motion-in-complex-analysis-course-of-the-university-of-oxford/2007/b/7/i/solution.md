<h1 id="b/7/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First, [planar Brownian motion](../../../../../planar-brownian-motion.md) started away from zero almost surely never hits zero. To see this without confusing it with neighborhood recurrence, stop in an [annulus](../../../../../annulus-mathematics.md) with inner radius $\epsilon$ and fixed outer radius $R>|Z_0|$. The preceding logarithmic calculation gives probability $\log(R/|Z_0|)/\log(R/\epsilon)$ of reaching the inner circle first. A hit of zero before the outer exit would require all these inner hits, so its probability is zero as $\epsilon\downarrow0$. On every finite path interval the continuous path is bounded; a countable union over integer outer radii and integer times proves the all-time assertion.

Consequently the [integrand](../../../../../integrand.md) $1/Z$ is locally square integrable: on every [compact](../../../../../compact-space.md) time interval the nonvanishing continuous path has a positive minimum modulus. Write $Z=X+iY$ with independent standard real coordinates. Complex [quadratic covariation](../../../../../quadratic-covariation.md) satisfies $d[Z,Z]=dt-dt+2i\,d[X,Y]=0$, so analytic [Itô's lemma](../../../../../ito-s-lemma.md) has no second-derivative drift. For $L=\int Z^{-1}dZ$ one likewise has $d[L,L]=0$, and $d[e^{-L},Z]=0$. The product rule therefore gives

$$
d(Z_te^{-L_t})=e^{-L_t}dZ_t-Z_te^{-L_t}dL_t=0.
$$

Its initial value is $Z_0$, proving, simultaneously for all times by [continuity](../../../../../continuous-function.md),

$$
\boxed{Z_t=Z_0e^{L_t}.}
$$

Thus $\Re L_t=\log(|Z_t|/|Z_0|)$ and $\Im L_t$ is the **continuous accumulated change of [complex argument](../../../../../argument-complex-analysis.md)** of the path about zero, measured in radians. It is a winding angle, without reduction modulo $2\pi$. A single-valued [logarithm](../../../../../logarithm.md) on the whole punctured plane is unnecessary; the path has a [continuous stochastic logarithm of planar Brownian motion](../../../../../continuous-stochastic-logarithm-of-planar-brownian-motion.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
