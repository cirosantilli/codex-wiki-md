<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

The equation is a [conservation law](../../../../../conservation-law.md) $n_t+J_x=0$ with [diffusive flux](../../../../../diffusive-flux.md) $J=-D(n_0/n)n_x$. For positive density, insects move down the density gradient, with effective [diffusion coefficient](../../../../../diffusion-coefficient.md) $Dn_0/n$: dispersal is stronger in low-density regions. This is [logarithmic diffusion](../../../../../logarithmic-diffusion.md), since the equation is $n_t=Dn_0(\log n)_{xx}$.

Put $\tau=Dt$ and $\xi=x/\tau^\beta$. A [self-similar solution](../../../../../similarity-solution.md) $n=n_0\tau^{-\beta}g(\xi)$ conserves total number when $\int_{\mathbb R}g=1$. Its width shrinks to zero as $t\downarrow0$; for an integrable nonnegative $g$, changing variables in the integral against a bounded [continuous function](../../../../../continuous-function.md) proves convergence to $n_0$ times the [Dirac delta distribution](../../../../../dirac-delta-function.md) at the origin.

Substitution gives

$$
-\beta\tau^{-\beta-1}(g+\xi g')
=\tau^{-2\beta}(g'/g)'.
$$

Matching powers for a nonstationary profile forces **$\beta=1$**. The profile equation integrates to $g'/g=-\xi g+C$. For a centred even profile, $C=0$, and integration of $g'=-\xi g^2$ gives $g=2/(\xi^2+a^2)$. Normalization requires $2\pi/a=1$, hence

$$
\boxed{g(\xi)=\frac2{\xi^2+4\pi^2},\qquad
n(x,t)=\frac{2n_0Dt}{x^2+4\pi^2D^2t^2}.}
$$

This is $n_0$ times a [Cauchy distribution](../../../../../cauchy-distribution.md) density with scale $2\pi Dt$. It is positive, has total mass $n_0$, and directly satisfies the [nonlinear diffusion equation](../../../../../nonlinear-diffusion-equation.md) for $t>0$.

## ↑ Ancestors (11)

1. [6B](../6b.md)
2. [Section I](../section-i.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
