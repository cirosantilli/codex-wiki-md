<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At $\alpha=0$ the transverse coordinates are independent [Brownian motions](../../../../brownian-motion-split.md) with [diffusion coefficient](../../../../diffusion-coefficient.md) $D=1$. The [cylinder](../../../../cylinder-geometry.md) is infinitely long, so the axial coordinate cannot affect its first contact time. By [rotational invariance of Brownian motion](../../../../rotational-invariance-of-brownian-motion.md), the [mean first-passage time](../../../../mean-first-passage-time.md) $u$ depends only on the transverse [radius](../../../../radius.md) $\rho=\sqrt{x^2+y^2}$.

The [Kolmogorov backward equation](../../../../kolmogorov-backward-equation.md) for a [mean first-passage time](../../../../mean-first-passage-time.md) is $Lu=-1$. Here $L=\partial_x^2+\partial_y^2$, so the radial [boundary value problem](../../../../boundary-value-problem-split.md) is

$$
u''(\rho)+\frac1\rho u'(\rho)=-1\quad(0<\rho<R),
\qquad u(R)=0.
$$

The [absorbing boundary condition for a diffusion](../../../../absorbing-boundary-condition-for-a-diffusion.md) is imposed on the circular cross-section. At $\rho=0$, the solution must extend smoothly over the axis. Multiplying by $\rho$ and integrating gives

$$
(\rho u')'=-\rho,
\qquad u'=-\frac\rho2+\frac C\rho,
\qquad u=-\frac{\rho^2}4+C\log\rho+C_0.
$$

Smoothness at the axis excludes the [logarithm](../../../../logarithm.md) term, and $u(R)=0$ fixes $C_0=R^2/4$. Consequently

$$
\boxed{\tau(\widehat r_0)=\frac{R^2-\widehat r_0^{\,2}}4.}
$$

This also verifies the finiteness assumption behind the [Kolmogorov backward equation](../../../../kolmogorov-backward-equation.md). Let $T$ be the first contact time and apply the stopped [Itô formula](../../../../ito-s-lemma.md) to the bounded nonnegative function $u$ just obtained. Its bounded derivatives on the disk make the stopped [stochastic integral](../../../../stochastic-integral.md) a [martingale](../../../../martingale-split.md), giving

$$
\mathbb E(t\wedge T)=u(\widehat r_0)-\mathbb E u\bigl(\rho(t\wedge T)\bigr)\leq u(\widehat r_0).
$$

By [monotone convergence](../../../../monotone-convergence-theorem.md), $T$ has finite [expected value](../../../../expected-value-split.md); continuity and [dominated convergence](../../../../dominated-convergence-theorem.md) then make the final term vanish as $t\to\infty$. Hence $u(\widehat r_0)=\mathbb ET$. In particular, the [mean first-passage time](../../../../mean-first-passage-time.md) is $R^2/4$ on the axis and tends to zero at the adsorbing wall.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the stochastic modelling of biological processes course of the University of Oxford](../../../split.md)
5. [Stochastic modelling of biological processes course of the University of Oxford](../../../../stochastic-modelling-of-biological-processes-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
